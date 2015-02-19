

##PHP Mail form example


The code below is an example script to send an email message using the Pear package Mail. You will need to authenticate with your CloudSite email address and password. 


	 <?php
    	 require_once "Mail.php";
      
    	 $from = "Some Person <changeme@example.com>";
    	 $to = "Someone Else <changeme@example.com>";
    	 $subject = "Test";
    	 $body = "Testing, is this thing on?";
      
    	 $host = "mail.cloudsite.com";
    	 $username = "you@cloudsite.com";
    	 $password = "your-password";
      
    	 $headers = array ('From' => $from,
    	   'To' => $to,
    	   'Subject' => $subject);
    	 $smtp = Mail::factory('smtp',
    	   array ('host' => $host,
    	     'auth' => true,
    	     'username' => $username,
    	     'password' => $password));
    	  
    	 $mail = $smtp->send($to, $headers, $body);
      
    	 if (PEAR::isError($mail)) {
    	   echo("<p>" . $mail->getMessage() . "</p>");
    	  } else {
    	   echo("<p>Message successfully sent!</p>");
    	  }
	?>

You will need to change the code below in the form to match your CloudSite. Replace cloudsite with your cloudsite domain name. 


     $from = "Some Person <changeme@example.com>";
     $to = "Someone Else <changeme@example.com>";
     $subject = "Test";
     $body = "Testing, is this thing on?";
      
     $host = "mail.cloudsite.com";
     $username = "you@cloudsite.com";
     $password = "your-password";