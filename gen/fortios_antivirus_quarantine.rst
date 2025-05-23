:source: fortios_antivirus_quarantine.py

:orphan:

.. fortios_antivirus_quarantine:

fortios_antivirus_quarantine -- Configure quarantine options in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify antivirus feature and quarantine category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.15


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------
Supported Version Ranges: v6.0.0 -> v7.6.2


Parameters
----------


.. raw:: html

    <ul>
    <li> <span class="li-head">access_token</span> - Token-based authentication. Generated from GUI of Fortigate. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> </li>
    <li> <span class="li-head">enable_log</span> - Enable/Disable logging for task. <span class="li-normal">type: bool</span> <span class="li-required">required: false</span> <span class="li-normal">default: False</span> </li>
    <li> <span class="li-head">vdom</span> - Virtual domain, among those defined previously. A vdom is a virtual instance of the FortiGate that can be configured and used as a different unit. <span class="li-normal">type: str</span> <span class="li-normal">default: root</span> </li>
    <li> <span class="li-head">member_path</span> - Member attribute path to operate on. <span class="li-normal">type: str</span> </li>
    <li> <span class="li-head">member_state</span> - Add or delete a member under specified attribute path. <span class="li-normal">type: str</span> <span class="li-normal">choices: present, absent</span> </li>
    <li> <span class="li-head">antivirus_quarantine</span> - Configure quarantine options. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>antivirus_quarantine</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">agelimit</span> - Age limit for quarantined files (0 - 479 hours, 0 means forever). <span class="li-normal">type: int</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>agelimit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">destination</span> - Choose whether to quarantine files to the FortiGate disk or to FortiAnalyzer or to delete them instead of quarantining them. <span class="li-normal">type: str</span> <span class="li-normal">choices: NULL, disk, FortiAnalyzer</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>destination</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[NULL]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[disk]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[FortiAnalyzer]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">drop_blocked</span> - Do not quarantine dropped files found in sessions using the selected protocols. Dropped files are deleted instead of being quarantined. <span class="li-normal">type: list</span> <span class="li-normal">choices: imap, smtp, pop3, http, ftp, nntp, imaps, smtps, pop3s, https, ftps, mapi, cifs, ssh, mm1, mm3, mm4, mm7</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>drop_blocked</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.0 </code></td>
 </tr>
 <tr>
 <td>[imap]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.0</code></td>
 <tr>
 <td>[smtp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.0</code></td>
 <tr>
 <td>[pop3]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.0</code></td>
 <tr>
 <td>[http]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.0</code></td>
 <tr>
 <td>[ftp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.0</code></td>
 <tr>
 <td>[nntp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.0</code></td>
 <tr>
 <td>[imaps]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.0</code></td>
 <tr>
 <td>[smtps]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.0</code></td>
 <tr>
 <td>[pop3s]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.0</code></td>
 <tr>
 <td>[https]</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.0</code></td>
 </tr>
 <tr>
 <td>[ftps]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.0</code></td>
 <tr>
 <td>[mapi]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.0</code></td>
 <tr>
 <td>[cifs]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.0</code></td>
 <tr>
 <td>[ssh]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.4.0</code></td>
 </tr>
 <tr>
 <td>[mm1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </tr>
 <tr>
 <td>[mm3]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </tr>
 <tr>
 <td>[mm4]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </tr>
 <tr>
 <td>[mm7]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">drop_heuristic</span> - Do not quarantine files detected by heuristics found in sessions using the selected protocols. Dropped files are deleted instead of being quarantined. <span class="li-normal">type: list</span> <span class="li-normal">choices: imap, smtp, pop3, http, ftp, nntp, imaps, smtps, pop3s, https, ftps, mapi, cifs, ssh, mm1, mm3, mm4, mm7</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>drop_heuristic</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0 </code></td>
 </tr>
 <tr>
 <td>[imap]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[smtp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[pop3]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[http]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[ftp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[nntp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[imaps]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[smtps]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[pop3s]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[https]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[ftps]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[mapi]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[cifs]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[ssh]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.0</code></td>
 </tr>
 <tr>
 <td>[mm1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </tr>
 <tr>
 <td>[mm3]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </tr>
 <tr>
 <td>[mm4]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </tr>
 <tr>
 <td>[mm7]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">drop_infected</span> - Do not quarantine infected files found in sessions using the selected protocols. Dropped files are deleted instead of being quarantined. <span class="li-normal">type: list</span> <span class="li-normal">choices: imap, smtp, pop3, http, ftp, nntp, imaps, smtps, pop3s, https, ftps, mapi, cifs, ssh, mm1, mm3, mm4, mm7</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>drop_infected</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[imap]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[smtp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[pop3]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[http]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[ftp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[nntp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[imaps]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[smtps]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[pop3s]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[https]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[ftps]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[mapi]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[cifs]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[ssh]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 </tr>
 <tr>
 <td>[mm1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </tr>
 <tr>
 <td>[mm3]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </tr>
 <tr>
 <td>[mm4]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </tr>
 <tr>
 <td>[mm7]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">drop_intercepted</span> - drop intercepted from a protocol <span class="li-normal">type: list</span> <span class="li-normal">choices: imap, smtp, pop3, http, ftp, imaps, smtps, pop3s, https, ftps, mapi, mm1, mm3, mm4, mm7</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>drop_intercepted</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[imap]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[smtp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[pop3]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[http]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[ftp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[imaps]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[smtps]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[pop3s]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[https]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[ftps]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[mapi]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[mm1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[mm3]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[mm4]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[mm7]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">drop_machine_learning</span> - Do not quarantine files detected by machine learning found in sessions using the selected protocols. Dropped files are deleted instead of being quarantined. <span class="li-normal">type: list</span> <span class="li-normal">choices: imap, smtp, pop3, http, ftp, nntp, imaps, smtps, pop3s, https, ftps, mapi, cifs, ssh</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>drop_machine_learning</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[imap]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[smtp]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[pop3]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[http]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[ftp]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[nntp]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[imaps]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[smtps]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[pop3s]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[https]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[ftps]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[mapi]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[cifs]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[ssh]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">lowspace</span> - Select the method for handling additional files when running low on disk space. <span class="li-normal">type: str</span> <span class="li-normal">choices: drop-new, ovrw-old</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>lowspace</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[drop-new]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[ovrw-old]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">maxfilesize</span> - Maximum file size to quarantine (0 - 500 Mbytes, 0 means unlimited). <span class="li-normal">type: int</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>maxfilesize</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">quarantine_quota</span> - The amount of disk space to reserve for quarantining files (0 - 4294967295 Mbytes, 0 means unlimited and depends on disk space). <span class="li-normal">type: int</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>quarantine_quota</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">store_blocked</span> - Quarantine blocked files found in sessions using the selected protocols. <span class="li-normal">type: list</span> <span class="li-normal">choices: imap, smtp, pop3, http, ftp, nntp, imaps, smtps, pop3s, https, ftps, mapi, cifs, ssh, mm1, mm3, mm4, mm7</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>store_blocked</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.0 </code></td>
 </tr>
 <tr>
 <td>[imap]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.0</code></td>
 <tr>
 <td>[smtp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.0</code></td>
 <tr>
 <td>[pop3]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.0</code></td>
 <tr>
 <td>[http]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.0</code></td>
 <tr>
 <td>[ftp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.0</code></td>
 <tr>
 <td>[nntp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.0</code></td>
 <tr>
 <td>[imaps]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.0</code></td>
 <tr>
 <td>[smtps]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.0</code></td>
 <tr>
 <td>[pop3s]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.0</code></td>
 <tr>
 <td>[https]</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.0</code></td>
 </tr>
 <tr>
 <td>[ftps]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.0</code></td>
 <tr>
 <td>[mapi]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.0</code></td>
 <tr>
 <td>[cifs]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.0</code></td>
 <tr>
 <td>[ssh]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.4.0</code></td>
 </tr>
 <tr>
 <td>[mm1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </tr>
 <tr>
 <td>[mm3]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </tr>
 <tr>
 <td>[mm4]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </tr>
 <tr>
 <td>[mm7]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">store_heuristic</span> - Quarantine files detected by heuristics found in sessions using the selected protocols. <span class="li-normal">type: list</span> <span class="li-normal">choices: imap, smtp, pop3, http, ftp, nntp, imaps, smtps, pop3s, https, ftps, mapi, cifs, ssh, mm1, mm3, mm4, mm7</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>store_heuristic</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0 </code></td>
 </tr>
 <tr>
 <td>[imap]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[smtp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[pop3]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[http]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[ftp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[nntp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[imaps]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[smtps]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[pop3s]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[https]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[ftps]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[mapi]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[cifs]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[ssh]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.0</code></td>
 </tr>
 <tr>
 <td>[mm1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </tr>
 <tr>
 <td>[mm3]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </tr>
 <tr>
 <td>[mm4]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </tr>
 <tr>
 <td>[mm7]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">store_infected</span> - Quarantine infected files found in sessions using the selected protocols. <span class="li-normal">type: list</span> <span class="li-normal">choices: imap, smtp, pop3, http, ftp, nntp, imaps, smtps, pop3s, https, ftps, mapi, cifs, ssh, mm1, mm3, mm4, mm7</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>store_infected</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[imap]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[smtp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[pop3]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[http]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[ftp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[nntp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[imaps]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[smtps]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[pop3s]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[https]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[ftps]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[mapi]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[cifs]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[ssh]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 </tr>
 <tr>
 <td>[mm1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </tr>
 <tr>
 <td>[mm3]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </tr>
 <tr>
 <td>[mm4]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </tr>
 <tr>
 <td>[mm7]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">store_intercepted</span> - quarantine intercepted from a protocol <span class="li-normal">type: list</span> <span class="li-normal">choices: imap, smtp, pop3, http, ftp, imaps, smtps, pop3s, https, ftps, mapi, mm1, mm3, mm4, mm7</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>store_intercepted</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[imap]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[smtp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[pop3]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[http]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[ftp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[imaps]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[smtps]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[pop3s]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[https]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[ftps]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[mapi]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[mm1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[mm3]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[mm4]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[mm7]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">store_machine_learning</span> - Quarantine files detected by machine learning found in sessions using the selected protocols. <span class="li-normal">type: list</span> <span class="li-normal">choices: imap, smtp, pop3, http, ftp, nntp, imaps, smtps, pop3s, https, ftps, mapi, cifs, ssh</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>store_machine_learning</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[imap]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[smtp]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[pop3]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[http]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[ftp]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[nntp]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[imaps]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[smtps]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[pop3s]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[https]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[ftps]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[mapi]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[cifs]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[ssh]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        </ul>
    </ul>


Notes
-----

.. note::

   - Legacy fortiosapi has been deprecated, httpapi is the preferred way to run playbooks

   - The module supports check_mode.



Examples
--------

.. code-block:: yaml+jinja
    
    - name: Configure quarantine options.
      fortinet.fortios.fortios_antivirus_quarantine:
          vdom: "{{ vdom }}"
          antivirus_quarantine:
              agelimit: "0"
              destination: "NULL"
              drop_blocked: "imap"
              drop_heuristic: "imap"
              drop_infected: "imap"
              drop_intercepted: "imap"
              drop_machine_learning: "imap"
              lowspace: "drop-new"
              maxfilesize: "0"
              quarantine_quota: "0"
              store_blocked: "imap"
              store_heuristic: "imap"
              store_infected: "imap"
              store_intercepted: "imap"
              store_machine_learning: "imap"


Return Values
-------------
Common return values are documented: https://docs.ansible.com/ansible/latest/reference_appendices/common_return_values.html#common-return-values, the following are the fields unique to this module:

.. raw:: html

    <ul>

    <li> <span class="li-return">build</span> - Build number of the fortigate image <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: 1547</span></li>
    <li> <span class="li-return">http_method</span> - Last method used to provision the content into FortiGate <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: PUT</span></li>
    <li> <span class="li-return">http_status</span> - Last result given by FortiGate on last operation applied <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: 200</span></li>
    <li> <span class="li-return">mkey</span> - Master key (id) used in the last call to FortiGate <span class="li-normal">returned: success</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: id</span></li>
    <li> <span class="li-return">name</span> - Name of the table used to fulfill the request <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: urlfilter</span></li>
    <li> <span class="li-return">path</span> - Path of the table used to fulfill the request <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: webfilter</span></li>
    <li> <span class="li-return">revision</span> - Internal revision number <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: 17.0.2.10658</span></li>
    <li> <span class="li-return">serial</span> - Serial number of the unit <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: FGVMEVYYQT3AB5352</span></li>
    <li> <span class="li-return">status</span> - Indication of the operation's result <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: success</span></li>
    <li> <span class="li-return">vdom</span> - Virtual domain used <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: root</span></li>
    <li> <span class="li-return">version</span> - Version of the FortiGate <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: v5.6.3</span></li>
    </ul>

Status
------

- This module is not guaranteed to have a backwards compatible interface.


Authors
-------

- Link Zheng (@chillancezen)
- Jie Xue (@JieX19)
- Hongbin Lu (@fgtdev-hblu)
- Frank Shen (@frankshen01)
- Miguel Angel Munoz (@mamunozgonzalez)
- Nicolas Thomas (@thomnico)


.. hint::
    If you notice any issues in this documentation, you can create a pull request to improve it.
