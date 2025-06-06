:source: fortios_wireless_controller_log.py

:orphan:

.. fortios_wireless_controller_log:

fortios_wireless_controller_log -- Configure wireless controller event log filters in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify wireless_controller feature and log category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.15


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------
Supported Version Ranges: v6.2.0 -> v7.6.2


Parameters
----------


.. raw:: html

    <ul>
    <li> <span class="li-head">access_token</span> - Token-based authentication. Generated from GUI of Fortigate. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> </li>
    <li> <span class="li-head">enable_log</span> - Enable/Disable logging for task. <span class="li-normal">type: bool</span> <span class="li-required">required: false</span> <span class="li-normal">default: False</span> </li>
    <li> <span class="li-head">vdom</span> - Virtual domain, among those defined previously. A vdom is a virtual instance of the FortiGate that can be configured and used as a different unit. <span class="li-normal">type: str</span> <span class="li-normal">default: root</span> </li>
    <li> <span class="li-head">member_path</span> - Member attribute path to operate on. <span class="li-normal">type: str</span> </li>
    <li> <span class="li-head">member_state</span> - Add or delete a member under specified attribute path. <span class="li-normal">type: str</span> <span class="li-normal">choices: present, absent</span> </li>
    <li> <span class="li-head">wireless_controller_log</span> - Configure wireless controller event log filters. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>wireless_controller_log</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">addrgrp_log</span> - Lowest severity level to log address group message. <span class="li-normal">type: str</span> <span class="li-normal">choices: emergency, alert, critical, error, warning, notification, information, debug</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>addrgrp_log</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[emergency]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[alert]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[critical]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[error]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[warning]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[notification]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[information]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[debug]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ble_log</span> - Lowest severity level to log BLE detection message. <span class="li-normal">type: str</span> <span class="li-normal">choices: emergency, alert, critical, error, warning, notification, information, debug</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ble_log</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[emergency]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[alert]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[critical]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[error]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[warning]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[notification]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[information]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[debug]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">clb_log</span> - Lowest severity level to log client load balancing message. <span class="li-normal">type: str</span> <span class="li-normal">choices: emergency, alert, critical, error, warning, notification, information, debug</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>clb_log</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[emergency]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[alert]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[critical]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[error]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[warning]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[notification]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[information]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[debug]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dhcp_starv_log</span> - Lowest severity level to log DHCP starvation event message. <span class="li-normal">type: str</span> <span class="li-normal">choices: emergency, alert, critical, error, warning, notification, information, debug</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dhcp_starv_log</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[emergency]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[alert]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[critical]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[error]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[warning]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[notification]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[information]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[debug]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">led_sched_log</span> - Lowest severity level to log LED schedule event message. <span class="li-normal">type: str</span> <span class="li-normal">choices: emergency, alert, critical, error, warning, notification, information, debug</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>led_sched_log</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[emergency]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[alert]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[critical]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[error]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[warning]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[notification]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[information]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[debug]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">radio_event_log</span> - Lowest severity level to log radio event message. <span class="li-normal">type: str</span> <span class="li-normal">choices: emergency, alert, critical, error, warning, notification, information, debug</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>radio_event_log</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[emergency]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[alert]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[critical]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[error]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[warning]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[notification]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[information]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[debug]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">rogue_event_log</span> - Lowest severity level to log rogue AP event message. <span class="li-normal">type: str</span> <span class="li-normal">choices: emergency, alert, critical, error, warning, notification, information, debug</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>rogue_event_log</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[emergency]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[alert]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[critical]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[error]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[warning]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[notification]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[information]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[debug]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">sta_event_log</span> - Lowest severity level to log station event message. <span class="li-normal">type: str</span> <span class="li-normal">choices: emergency, alert, critical, error, warning, notification, information, debug</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sta_event_log</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[emergency]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[alert]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[critical]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[error]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[warning]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[notification]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[information]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[debug]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">sta_locate_log</span> - Lowest severity level to log station locate message. <span class="li-normal">type: str</span> <span class="li-normal">choices: emergency, alert, critical, error, warning, notification, information, debug</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sta_locate_log</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[emergency]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[alert]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[critical]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[error]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[warning]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[notification]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[information]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[debug]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">status</span> - Enable/disable wireless event logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">wids_log</span> - Lowest severity level to log WIDS message. <span class="li-normal">type: str</span> <span class="li-normal">choices: emergency, alert, critical, error, warning, notification, information, debug</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>wids_log</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[emergency]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[alert]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[critical]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[error]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[warning]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[notification]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[information]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[debug]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">wtp_event_log</span> - Lowest severity level to log WTP event message. <span class="li-normal">type: str</span> <span class="li-normal">choices: emergency, alert, critical, error, warning, notification, information, debug</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>wtp_event_log</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[emergency]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[alert]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[critical]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[error]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[warning]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[notification]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[information]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[debug]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">wtp_fips_event_log</span> - Lowest severity level to log FAP fips event message. <span class="li-normal">type: str</span> <span class="li-normal">choices: emergency, alert, critical, error, warning, notification, information, debug</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>wtp_fips_event_log</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[emergency]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.2</code></td>
 <tr>
 <td>[alert]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.2</code></td>
 <tr>
 <td>[critical]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.2</code></td>
 <tr>
 <td>[error]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.2</code></td>
 <tr>
 <td>[warning]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.2</code></td>
 <tr>
 <td>[notification]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.2</code></td>
 <tr>
 <td>[information]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.2</code></td>
 <tr>
 <td>[debug]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.2</code></td>
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
    
    - name: Configure wireless controller event log filters.
      fortinet.fortios.fortios_wireless_controller_log:
          vdom: "{{ vdom }}"
          wireless_controller_log:
              addrgrp_log: "emergency"
              ble_log: "emergency"
              clb_log: "emergency"
              dhcp_starv_log: "emergency"
              led_sched_log: "emergency"
              radio_event_log: "emergency"
              rogue_event_log: "emergency"
              sta_event_log: "emergency"
              sta_locate_log: "emergency"
              status: "enable"
              wids_log: "emergency"
              wtp_event_log: "emergency"
              wtp_fips_event_log: "emergency"


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
