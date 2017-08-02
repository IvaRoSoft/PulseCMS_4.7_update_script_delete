# PulseCMS_4.7_update_script_delete
Upravený skript: admin/inc/delete.php

Riešenie:

V PulseCMS 4.7 je v niektorých prípadoch problem s odtraňovaním

jednotlivých obrázkov respektíve celých galérií.

Ako upraviť:

Stiahnite si skript delete-update.php.

Vytvorte zálohu skriptu v admin/inc/delete.php.

Nahrajte a premenujte skript delete-update.php.

Upravené riadky (3 riadky) od 25

-------------------------
<pre>
// My code, 3 rows
$undir = "../content/".$del[0].'/'.$del[1];
//unlink($opFile);
 rmdir($undir);	
// end My code
</pre>
---------------------
Help:

http://php.net/manual/en/function.rmdir.php

http://php.net/manual/en/function.unlink.php

IvaRo
