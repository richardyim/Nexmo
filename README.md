Nexmo
=====

Nexmo Test File
$sms = new NexmoMessage('account_key', 'account_secret');
    $sms->sendText( '+16508631789', 'MyApp', 'Hello world!' );
