# Overriding Connection Strings on Octane

The connection strings in the Portal allow you to override existing connection strings which are already defined in the **web.config**. If your web.config does not contain a connection string with the same name as the one configured in the portal, it will not be added and be accessible at run time. This might be the issue you're experiencing.

A GearHost CloudSite does not physically modify the **web.config** (source), it does this at run time. So in order to check which **AppSettings** and **ConnectionStrings** are actually available at run time, try this:

>Controller:

```
public ActionResult Index()
{
  ViewBag.ConnectionStrings =
    ConfigurationManager.ConnectionStrings.Cast<ConnectionStringSettings>();
  ViewBag.AppSettings = ConfigurationManager.AppSettings;
  return View();
}
```
>View:

```
<h3>ConnectionStrings:</h3>
<ul>
  @foreach (var setting in ViewBag.ConnectionStrings)
  {
    <li>@setting.Name: @setting.ConnectionString</li>
  }
</ul>
<h3>AppSettings:</h3>
<ul>
  @foreach (var s in ViewBag.AppSettings)
  {
    <li>@setting: @System.Configuration.ConfigurationManager.AppSettings[s]</li>
  }
</ul>
```

The following can be used in a Web Forms page using Model Binding.

>GridView:

```
<asp:GridView ID="GridView1" runat="server"
	ItemName="System.Configuration.ConnectionStringSettingsCollection"
	SelectMethod="GridView1_GetData" />
```

>SelectMethod:

```
public IEnumerable<ConnectionStringSettings> GridView1_GetData()
{
    return ConfigurationManager.ConnectionStrings.Cast<ConnectionStringSettings>(); ;
}
```
