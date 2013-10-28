Nexmo
=====

Nexmo Test File
$sms = new NexmoMessage('99010bdb', '38ed90fe');
    $sms->sendText( '+16508631789', 'MyApp', 'Hello world!' );
    
    $receipt = new NexmoReceipt();
     if ($receipt->exists()) {
         switch ($receipt->status) {
             case $receipt::STATUS_DELIVERED:
                 // The message was delivered to the handset!
                 break;
             
             case $receipt::STATUS_FAILED:
             case $receipt::STATUS_EXPIRED:
                 // The message failed to be delivered
                 break;
         }
     }
