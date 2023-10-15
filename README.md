# phpmailer
Send email using phpmailer <br>
open index.php and modify : <br>
//Define smtp host line no 24<br>
	$mail->Host = "smtp.gmail.com";<br>
//Port to connect smtp line no 30 <br>
	$mail->Port = "587"; <br>
//Set gmail username line no 32 <br>
	$mail->Username = "Your Gmail Email Address Here"; <br>
//Set gmail password line no 34  <br>
	$mail->Password = "Your Gmail Password Here"; <br>
//Set sender email line no 38 <br>
	$mail->setFrom('Sender Email who will send email'); <br>
//Enable HTML <br>
	$mail->isHTML(true); <br>
//Attachment <br>
	$mail->addAttachment('img/attachment.png'); <br>
//Email body <br>
	$mail->Body = "<h1>This is HTML h1 Heading</h1></br><p>This is html paragraph</p>"; <br>
//Add recipient line no 45 <br>
	$mail->addAddress('Email of the person who will receive email');
