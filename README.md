# phpmailer
Send email using phpmailer
open index.php and modify : 
//Define smtp host line no 24
	$mail->Host = "smtp.gmail.com";
//Port to connect smtp line no 30
	$mail->Port = "587";
//Set gmail username line no 32
	$mail->Username = "Your Gmail Email Address Here";
//Set gmail password line no 34 
	$mail->Password = "Your Gmail Password Here";
//Set sender email line no 38
	$mail->setFrom('Sender Email who will send email');
//Enable HTML
	$mail->isHTML(true);
//Attachment
	$mail->addAttachment('img/attachment.png');
//Email body
	$mail->Body = "<h1>This is HTML h1 Heading</h1></br><p>This is html paragraph</p>";
//Add recipient line no 45
	$mail->addAddress('Email of the person who will receive email');
