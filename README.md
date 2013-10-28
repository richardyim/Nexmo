Nexmo
=====

Nexmo Test File
$sms = new NexmoMessage('99010bdb', '38ed90fe');
    $sms->sendText( '+16508631789', 'MyApp', 'Hello world!' );
