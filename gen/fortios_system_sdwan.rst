:source: fortios_system_sdwan.py

:orphan:

.. fortios_system_sdwan:

fortios_system_sdwan -- Configure redundant Internet connections with multiple outbound links and health-check profiles in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and sdwan category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.15


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------
Supported Version Ranges: v6.4.0 -> v7.6.2


Parameters
----------


.. raw:: html

    <ul>
    <li> <span class="li-head">access_token</span> - Token-based authentication. Generated from GUI of Fortigate. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> </li>
    <li> <span class="li-head">enable_log</span> - Enable/Disable logging for task. <span class="li-normal">type: bool</span> <span class="li-required">required: false</span> <span class="li-normal">default: False</span> </li>
    <li> <span class="li-head">vdom</span> - Virtual domain, among those defined previously. A vdom is a virtual instance of the FortiGate that can be configured and used as a different unit. <span class="li-normal">type: str</span> <span class="li-normal">default: root</span> </li>
    <li> <span class="li-head">member_path</span> - Member attribute path to operate on. <span class="li-normal">type: str</span> </li>
    <li> <span class="li-head">member_state</span> - Add or delete a member under specified attribute path. <span class="li-normal">type: str</span> <span class="li-normal">choices: present, absent</span> </li>
    <li> <span class="li-head">system_sdwan</span> - Configure redundant Internet connections with multiple outbound links and health-check profiles. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>system_sdwan</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">app_perf_log_period</span> - Time interval in seconds that application performance logs are generated (0 - 3600). <span class="li-normal">type: int</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>app_perf_log_period</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">duplication</span> - Create SD-WAN duplication rule. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: duplication:id</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>duplication</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">dstaddr</span> - Destination address or address group names. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: duplication:id/dstaddr:name</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dstaddr</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Address or address group name. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">dstaddr6</span> - Destination address6 or address6 group names. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: duplication:id/dstaddr6:name</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dstaddr6</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Address6 or address6 group name. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">dstintf</span> - Outgoing (egress) interfaces or zones. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: duplication:id/dstintf:name</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dstintf</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Interface, zone or SDWAN zone name. Source system.interface.name system.zone.name system.sdwan.zone.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">id</span> - Duplication rule ID (1 - 255). see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">packet_de_duplication</span> - Enable/disable discarding of packets that have been duplicated. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>packet_de_duplication</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">packet_duplication</span> - Configure packet duplication method. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, force, on-demand</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>packet_duplication</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <tr>
 <td>[force]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <tr>
 <td>[on-demand]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">service</span> - Service and service group name. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: duplication:id/service:name</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>service</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Service and service group name. Source firewall.service.custom.name firewall.service.group.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">service_id</span> - SD-WAN service rule ID list. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: duplication:id/service_id:id</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>service_id</td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">id</span> - SD-WAN service rule ID. see <a href='#notes'>Notes</a>. Source system.sdwan.service.id. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">sla_match_service</span> - Enable/disable packet duplication matching health-check SLAs in service rule. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sla_match_service</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">srcaddr</span> - Source address or address group names. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: duplication:id/srcaddr:name</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>srcaddr</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Address or address group name. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">srcaddr6</span> - Source address6 or address6 group names. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: duplication:id/srcaddr6:name</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>srcaddr6</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Address6 or address6 group name. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">srcintf</span> - Incoming (ingress) interfaces or zones. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: duplication:id/srcintf:name</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>srcintf</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Interface, zone or SDWAN zone name. Source system.interface.name system.zone.name system.sdwan.zone.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            </ul>
        <li> <span class="li-head">duplication_max_discrepancy</span> - Maximum discrepancy between two packets for deduplication in milliseconds (250 - 1000). <span class="li-normal">type: int</span>
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>duplication_max_discrepancy</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">duplication_max_num</span> - Maximum number of interface members a packet is duplicated in the SD-WAN zone (2 - 4). <span class="li-normal">type: int</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>duplication_max_num</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">fail_alert_interfaces</span> - Physical interfaces that will be alerted. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: fail_alert_interfaces:name</span>
 <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fail_alert_interfaces</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Physical interface name. Source system.interface.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">fail_detect</span> - Enable/disable SD-WAN Internet connection status checking (failure detection). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label54' href="javascript:ContentClick('label55', 'label54');" onmouseover="ContentPreview('label55');" onmouseout="ContentUnpreview('label55');" title="click to collapse or expand..."> more... </a>
 <div id="label55" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fail_detect</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">health_check</span> - SD-WAN status checking or health checking. Identify a server on the Internet and determine how SD-WAN verifies that the FortiGate can communicate with it. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: health_check:name</span>
 <a id='label56' href="javascript:ContentClick('label57', 'label56');" onmouseover="ContentPreview('label57');" onmouseout="ContentUnpreview('label57');" title="click to collapse or expand..."> more... </a>
 <div id="label57" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>health_check</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">addr_mode</span> - Address mode (IPv4 or IPv6). <span class="li-normal">type: str</span> <span class="li-normal">choices: ipv4, ipv6</span>
 <a id='label58' href="javascript:ContentClick('label59', 'label58');" onmouseover="ContentPreview('label59');" onmouseout="ContentUnpreview('label59');" title="click to collapse or expand..."> more... </a>
 <div id="label59" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>addr_mode</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[ipv4]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[ipv6]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">class_id</span> - Traffic class ID. Source firewall.traffic-class.class-id. <span class="li-normal">type: int</span>
 <a id='label60' href="javascript:ContentClick('label61', 'label60');" onmouseover="ContentPreview('label61');" onmouseout="ContentUnpreview('label61');" title="click to collapse or expand..."> more... </a>
 <div id="label61" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>class_id</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">detect_mode</span> - The mode determining how to detect the server. <span class="li-normal">type: str</span> <span class="li-normal">choices: active, passive, prefer-passive, remote, agent-based</span>
 <a id='label62' href="javascript:ContentClick('label63', 'label62');" onmouseover="ContentPreview('label63');" onmouseout="ContentUnpreview('label63');" title="click to collapse or expand..."> more... </a>
 <div id="label63" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>detect_mode</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[active]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[passive]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[prefer-passive]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[remote]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.2</code></td>
 </tr>
 <tr>
 <td>[agent-based]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.2</code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">diffservcode</span> - Differentiated services code point (DSCP) in the IP header of the probe packet. <span class="li-normal">type: str</span>
 <a id='label64' href="javascript:ContentClick('label65', 'label64');" onmouseover="ContentPreview('label65');" onmouseout="ContentUnpreview('label65');" title="click to collapse or expand..."> more... </a>
 <div id="label65" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>diffservcode</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">dns_match_ip</span> - Response IP expected from DNS server if the protocol is DNS. <span class="li-normal">type: str</span>
 <a id='label66' href="javascript:ContentClick('label67', 'label66');" onmouseover="ContentPreview('label67');" onmouseout="ContentUnpreview('label67');" title="click to collapse or expand..."> more... </a>
 <div id="label67" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dns_match_ip</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">dns_request_domain</span> - Fully qualified domain name to resolve for the DNS probe. <span class="li-normal">type: str</span>
 <a id='label68' href="javascript:ContentClick('label69', 'label68');" onmouseover="ContentPreview('label69');" onmouseout="ContentUnpreview('label69');" title="click to collapse or expand..."> more... </a>
 <div id="label69" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dns_request_domain</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">embed_measured_health</span> - Enable/disable embedding measured health information. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label70' href="javascript:ContentClick('label71', 'label70');" onmouseover="ContentPreview('label71');" onmouseout="ContentUnpreview('label71');" title="click to collapse or expand..."> more... </a>
 <div id="label71" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>embed_measured_health</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">failtime</span> - Number of failures before server is considered lost (1 - 3600). <span class="li-normal">type: int</span>
 <a id='label72' href="javascript:ContentClick('label73', 'label72');" onmouseover="ContentPreview('label73');" onmouseout="ContentUnpreview('label73');" title="click to collapse or expand..."> more... </a>
 <div id="label73" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>failtime</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">fortiguard</span> - Enable/disable use of FortiGuard predefined server. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label74' href="javascript:ContentClick('label75', 'label74');" onmouseover="ContentPreview('label75');" onmouseout="ContentUnpreview('label75');" title="click to collapse or expand..."> more... </a>
 <div id="label75" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fortiguard</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.2</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">fortiguard_name</span> - Predefined health-check target name. Source system.health-check-fortiguard.name. <span class="li-normal">type: str</span>
 <a id='label76' href="javascript:ContentClick('label77', 'label76');" onmouseover="ContentPreview('label77');" onmouseout="ContentUnpreview('label77');" title="click to collapse or expand..."> more... </a>
 <div id="label77" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fortiguard_name</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ftp_file</span> - Full path and file name on the FTP server to download for FTP health-check to probe. <span class="li-normal">type: str</span>
 <a id='label78' href="javascript:ContentClick('label79', 'label78');" onmouseover="ContentPreview('label79');" onmouseout="ContentUnpreview('label79');" title="click to collapse or expand..."> more... </a>
 <div id="label79" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ftp_file</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ftp_mode</span> - FTP mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: passive, port</span>
 <a id='label80' href="javascript:ContentClick('label81', 'label80');" onmouseover="ContentPreview('label81');" onmouseout="ContentUnpreview('label81');" title="click to collapse or expand..."> more... </a>
 <div id="label81" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ftp_mode</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[passive]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <tr>
 <td>[port]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ha_priority</span> - HA election priority (1 - 50). <span class="li-normal">type: int</span>
 <a id='label82' href="javascript:ContentClick('label83', 'label82');" onmouseover="ContentPreview('label83');" onmouseout="ContentUnpreview('label83');" title="click to collapse or expand..."> more... </a>
 <div id="label83" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ha_priority</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">http_agent</span> - String in the http-agent field in the HTTP header. <span class="li-normal">type: str</span>
 <a id='label84' href="javascript:ContentClick('label85', 'label84');" onmouseover="ContentPreview('label85');" onmouseout="ContentUnpreview('label85');" title="click to collapse or expand..."> more... </a>
 <div id="label85" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>http_agent</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">http_get</span> - URL used to communicate with the server if the protocol if the protocol is HTTP. <span class="li-normal">type: str</span>
 <a id='label86' href="javascript:ContentClick('label87', 'label86');" onmouseover="ContentPreview('label87');" onmouseout="ContentUnpreview('label87');" title="click to collapse or expand..."> more... </a>
 <div id="label87" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>http_get</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">http_match</span> - Response string expected from the server if the protocol is HTTP. <span class="li-normal">type: str</span>
 <a id='label88' href="javascript:ContentClick('label89', 'label88');" onmouseover="ContentPreview('label89');" onmouseout="ContentUnpreview('label89');" title="click to collapse or expand..."> more... </a>
 <div id="label89" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>http_match</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">interval</span> - Status check interval in milliseconds, or the time between attempting to connect to the server (20 - 3600*1000 msec). <span class="li-normal">type: int</span>
 <a id='label90' href="javascript:ContentClick('label91', 'label90');" onmouseover="ContentPreview('label91');" onmouseout="ContentUnpreview('label91');" title="click to collapse or expand..."> more... </a>
 <div id="label91" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>interval</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">members</span> - Member sequence number list. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: health_check:name/members:seq_num</span>
 <a id='label92' href="javascript:ContentClick('label93', 'label92');" onmouseover="ContentPreview('label93');" onmouseout="ContentUnpreview('label93');" title="click to collapse or expand..."> more... </a>
 <div id="label93" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>members</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">seq_num</span> - Member sequence number. see <a href='#notes'>Notes</a>. Source system.sdwan.members.seq-num. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label94' href="javascript:ContentClick('label95', 'label94');" onmouseover="ContentPreview('label95');" onmouseout="ContentUnpreview('label95');" title="click to collapse or expand..."> more... </a>
 <div id="label95" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>seq_num</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">mos_codec</span> - Codec to use for MOS calculation . <span class="li-normal">type: str</span> <span class="li-normal">choices: g711, g722, g729</span>
 <a id='label96' href="javascript:ContentClick('label97', 'label96');" onmouseover="ContentPreview('label97');" onmouseout="ContentUnpreview('label97');" title="click to collapse or expand..."> more... </a>
 <div id="label97" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mos_codec</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[g711]</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[g722]</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[g729]</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">name</span> - Status check or health check name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label98' href="javascript:ContentClick('label99', 'label98');" onmouseover="ContentPreview('label99');" onmouseout="ContentUnpreview('label99');" title="click to collapse or expand..."> more... </a>
 <div id="label99" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">packet_size</span> - Packet size of a TWAMP test session. (124/158 - 1024) <span class="li-normal">type: int</span>
 <a id='label100' href="javascript:ContentClick('label101', 'label100');" onmouseover="ContentPreview('label101');" onmouseout="ContentUnpreview('label101');" title="click to collapse or expand..."> more... </a>
 <div id="label101" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>packet_size</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">password</span> - TWAMP controller password in authentication mode. <span class="li-normal">type: str</span>
 <a id='label102' href="javascript:ContentClick('label103', 'label102');" onmouseover="ContentPreview('label103');" onmouseout="ContentUnpreview('label103');" title="click to collapse or expand..."> more... </a>
 <div id="label103" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>password</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">port</span> - Port number used to communicate with the server over the selected protocol (0 - 65535). <span class="li-normal">type: int</span>
 <a id='label104' href="javascript:ContentClick('label105', 'label104');" onmouseover="ContentPreview('label105');" onmouseout="ContentUnpreview('label105');" title="click to collapse or expand..."> more... </a>
 <div id="label105" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>port</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">probe_count</span> - Number of most recent probes that should be used to calculate latency and jitter (5 - 30). <span class="li-normal">type: int</span>
 <a id='label106' href="javascript:ContentClick('label107', 'label106');" onmouseover="ContentPreview('label107');" onmouseout="ContentUnpreview('label107');" title="click to collapse or expand..."> more... </a>
 <div id="label107" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>probe_count</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">probe_packets</span> - Enable/disable transmission of probe packets. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label108' href="javascript:ContentClick('label109', 'label108');" onmouseover="ContentPreview('label109');" onmouseout="ContentUnpreview('label109');" title="click to collapse or expand..."> more... </a>
 <div id="label109" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>probe_packets</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">probe_timeout</span> - Time to wait before a probe packet is considered lost (20 - 3600*1000 msec). <span class="li-normal">type: int</span>
 <a id='label110' href="javascript:ContentClick('label111', 'label110');" onmouseover="ContentPreview('label111');" onmouseout="ContentUnpreview('label111');" title="click to collapse or expand..."> more... </a>
 <div id="label111" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>probe_timeout</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">protocol</span> - Protocol used to determine if the FortiGate can communicate with the server. <span class="li-normal">type: str</span> <span class="li-normal">choices: ping, tcp-echo, udp-echo, http, https, twamp, dns, tcp-connect, ftp, ping6</span>
 <a id='label112' href="javascript:ContentClick('label113', 'label112');" onmouseover="ContentPreview('label113');" onmouseout="ContentUnpreview('label113');" title="click to collapse or expand..."> more... </a>
 <div id="label113" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>protocol</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[ping]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[tcp-echo]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[udp-echo]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[http]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[https]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2</code></td>
 </tr>
 <tr>
 <td>[twamp]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[dns]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[tcp-connect]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2</code></td>
 </tr>
 <tr>
 <td>[ftp]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2</code></td>
 </tr>
 <tr>
 <td>[ping6]</td>
 <td><code class="docutils literal notranslate">v6.4.1 -> v6.4.1</code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">quality_measured_method</span> - Method to measure the quality of tcp-connect. <span class="li-normal">type: str</span> <span class="li-normal">choices: half-open, half-close</span>
 <a id='label114' href="javascript:ContentClick('label115', 'label114');" onmouseover="ContentPreview('label115');" onmouseout="ContentUnpreview('label115');" title="click to collapse or expand..."> more... </a>
 <div id="label115" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>quality_measured_method</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[half-open]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <tr>
 <td>[half-close]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">recoverytime</span> - Number of successful responses received before server is considered recovered (1 - 3600). <span class="li-normal">type: int</span>
 <a id='label116' href="javascript:ContentClick('label117', 'label116');" onmouseover="ContentPreview('label117');" onmouseout="ContentUnpreview('label117');" title="click to collapse or expand..."> more... </a>
 <div id="label117" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>recoverytime</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">security_mode</span> - Twamp controller security mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, authentication</span>
 <a id='label118' href="javascript:ContentClick('label119', 'label118');" onmouseover="ContentPreview('label119');" onmouseout="ContentUnpreview('label119');" title="click to collapse or expand..."> more... </a>
 <div id="label119" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>security_mode</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[authentication]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">server</span> - IP address or FQDN name of the server. <span class="li-normal">type: list</span> </li>
            <li> <span class="li-head">sla</span> - Service level agreement (SLA). <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: health_check:name/sla:id</span>
 <a id='label120' href="javascript:ContentClick('label121', 'label120');" onmouseover="ContentPreview('label121');" onmouseout="ContentUnpreview('label121');" title="click to collapse or expand..."> more... </a>
 <div id="label121" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sla</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">id</span> - SLA ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label122' href="javascript:ContentClick('label123', 'label122');" onmouseover="ContentPreview('label123');" onmouseout="ContentUnpreview('label123');" title="click to collapse or expand..."> more... </a>
 <div id="label123" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">jitter_threshold</span> - Jitter for SLA to make decision in milliseconds. (0 - 10000000). <span class="li-normal">type: int</span>
 <a id='label124' href="javascript:ContentClick('label125', 'label124');" onmouseover="ContentPreview('label125');" onmouseout="ContentUnpreview('label125');" title="click to collapse or expand..."> more... </a>
 <div id="label125" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>jitter_threshold</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">latency_threshold</span> - Latency for SLA to make decision in milliseconds. (0 - 10000000). <span class="li-normal">type: int</span>
 <a id='label126' href="javascript:ContentClick('label127', 'label126');" onmouseover="ContentPreview('label127');" onmouseout="ContentUnpreview('label127');" title="click to collapse or expand..."> more... </a>
 <div id="label127" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>latency_threshold</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">link_cost_factor</span> - Criteria on which to base link selection. <span class="li-normal">type: list</span> <span class="li-normal">choices: latency, jitter, packet-loss, mos, remote</span>
 <a id='label128' href="javascript:ContentClick('label129', 'label128');" onmouseover="ContentPreview('label129');" onmouseout="ContentUnpreview('label129');" title="click to collapse or expand..."> more... </a>
 <div id="label129" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>link_cost_factor</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[latency]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[jitter]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[packet-loss]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[mos]</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> 7.6.2</code></td>
 </tr>
 <tr>
 <td>[remote]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.2</code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">mos_threshold</span> - Minimum Mean Opinion Score for SLA to be marked as pass. (1.0 - 5.0). <span class="li-normal">type: str</span>
 <a id='label130' href="javascript:ContentClick('label131', 'label130');" onmouseover="ContentPreview('label131');" onmouseout="ContentUnpreview('label131');" title="click to collapse or expand..."> more... </a>
 <div id="label131" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mos_threshold</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">packetloss_threshold</span> - Packet loss for SLA to make decision in percentage. (0 - 100). <span class="li-normal">type: int</span>
 <a id='label132' href="javascript:ContentClick('label133', 'label132');" onmouseover="ContentPreview('label133');" onmouseout="ContentUnpreview('label133');" title="click to collapse or expand..."> more... </a>
 <div id="label133" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>packetloss_threshold</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">priority_in_sla</span> - Value to be distributed into routing table when in-sla (0 - 65535). <span class="li-normal">type: int</span>
 <a id='label134' href="javascript:ContentClick('label135', 'label134');" onmouseover="ContentPreview('label135');" onmouseout="ContentUnpreview('label135');" title="click to collapse or expand..."> more... </a>
 <div id="label135" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>priority_in_sla</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">priority_out_sla</span> - Value to be distributed into routing table when out-sla (0 - 65535). <span class="li-normal">type: int</span>
 <a id='label136' href="javascript:ContentClick('label137', 'label136');" onmouseover="ContentPreview('label137');" onmouseout="ContentUnpreview('label137');" title="click to collapse or expand..."> more... </a>
 <div id="label137" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>priority_out_sla</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">sla_fail_log_period</span> - Time interval in seconds that SLA fail log messages will be generated (0 - 3600). <span class="li-normal">type: int</span>
 <a id='label138' href="javascript:ContentClick('label139', 'label138');" onmouseover="ContentPreview('label139');" onmouseout="ContentUnpreview('label139');" title="click to collapse or expand..."> more... </a>
 <div id="label139" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sla_fail_log_period</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">sla_id_redistribute</span> - Select the ID from the SLA sub-table. The selected SLA"s priority value will be distributed into the routing table (0 - 32). <span class="li-normal">type: int</span>
 <a id='label140' href="javascript:ContentClick('label141', 'label140');" onmouseover="ContentPreview('label141');" onmouseout="ContentUnpreview('label141');" title="click to collapse or expand..."> more... </a>
 <div id="label141" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sla_id_redistribute</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">sla_pass_log_period</span> - Time interval in seconds that SLA pass log messages will be generated (0 - 3600). <span class="li-normal">type: int</span>
 <a id='label142' href="javascript:ContentClick('label143', 'label142');" onmouseover="ContentPreview('label143');" onmouseout="ContentUnpreview('label143');" title="click to collapse or expand..."> more... </a>
 <div id="label143" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sla_pass_log_period</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">source</span> - Source IP address used in the health-check packet to the server. <span class="li-normal">type: str</span>
 <a id='label144' href="javascript:ContentClick('label145', 'label144');" onmouseover="ContentPreview('label145');" onmouseout="ContentUnpreview('label145');" title="click to collapse or expand..."> more... </a>
 <div id="label145" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>source</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">source6</span> - Source IPv6 address used in the health-check packet to server. <span class="li-normal">type: str</span>
 <a id='label146' href="javascript:ContentClick('label147', 'label146');" onmouseover="ContentPreview('label147');" onmouseout="ContentUnpreview('label147');" title="click to collapse or expand..."> more... </a>
 <div id="label147" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>source6</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">system_dns</span> - Enable/disable system DNS as the probe server. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label148' href="javascript:ContentClick('label149', 'label148');" onmouseover="ContentPreview('label149');" onmouseout="ContentUnpreview('label149');" title="click to collapse or expand..."> more... </a>
 <div id="label149" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>system_dns</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">threshold_alert_jitter</span> - Alert threshold for jitter (ms). <span class="li-normal">type: int</span>
 <a id='label150' href="javascript:ContentClick('label151', 'label150');" onmouseover="ContentPreview('label151');" onmouseout="ContentUnpreview('label151');" title="click to collapse or expand..."> more... </a>
 <div id="label151" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>threshold_alert_jitter</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">threshold_alert_latency</span> - Alert threshold for latency (ms). <span class="li-normal">type: int</span>
 <a id='label152' href="javascript:ContentClick('label153', 'label152');" onmouseover="ContentPreview('label153');" onmouseout="ContentUnpreview('label153');" title="click to collapse or expand..."> more... </a>
 <div id="label153" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>threshold_alert_latency</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">threshold_alert_packetloss</span> - Alert threshold for packet loss (percentage). <span class="li-normal">type: int</span>
 <a id='label154' href="javascript:ContentClick('label155', 'label154');" onmouseover="ContentPreview('label155');" onmouseout="ContentUnpreview('label155');" title="click to collapse or expand..."> more... </a>
 <div id="label155" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>threshold_alert_packetloss</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">threshold_warning_jitter</span> - Warning threshold for jitter (ms). <span class="li-normal">type: int</span>
 <a id='label156' href="javascript:ContentClick('label157', 'label156');" onmouseover="ContentPreview('label157');" onmouseout="ContentUnpreview('label157');" title="click to collapse or expand..."> more... </a>
 <div id="label157" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>threshold_warning_jitter</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">threshold_warning_latency</span> - Warning threshold for latency (ms). <span class="li-normal">type: int</span>
 <a id='label158' href="javascript:ContentClick('label159', 'label158');" onmouseover="ContentPreview('label159');" onmouseout="ContentUnpreview('label159');" title="click to collapse or expand..."> more... </a>
 <div id="label159" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>threshold_warning_latency</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">threshold_warning_packetloss</span> - Warning threshold for packet loss (percentage). <span class="li-normal">type: int</span>
 <a id='label160' href="javascript:ContentClick('label161', 'label160');" onmouseover="ContentPreview('label161');" onmouseout="ContentUnpreview('label161');" title="click to collapse or expand..."> more... </a>
 <div id="label161" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>threshold_warning_packetloss</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">update_cascade_interface</span> - Enable/disable update cascade interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label162' href="javascript:ContentClick('label163', 'label162');" onmouseover="ContentPreview('label163');" onmouseout="ContentUnpreview('label163');" title="click to collapse or expand..."> more... </a>
 <div id="label163" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>update_cascade_interface</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">update_static_route</span> - Enable/disable updating the static route. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label164' href="javascript:ContentClick('label165', 'label164');" onmouseover="ContentPreview('label165');" onmouseout="ContentUnpreview('label165');" title="click to collapse or expand..."> more... </a>
 <div id="label165" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>update_static_route</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">user</span> - The user name to access probe server. <span class="li-normal">type: str</span>
 <a id='label166' href="javascript:ContentClick('label167', 'label166');" onmouseover="ContentPreview('label167');" onmouseout="ContentUnpreview('label167');" title="click to collapse or expand..."> more... </a>
 <div id="label167" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>user</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">vrf</span> - Virtual Routing Forwarding ID. <span class="li-normal">type: int</span>
 <a id='label168' href="javascript:ContentClick('label169', 'label168');" onmouseover="ContentPreview('label169');" onmouseout="ContentUnpreview('label169');" title="click to collapse or expand..."> more... </a>
 <div id="label169" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vrf</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">health_check_fortiguard</span> - SD-WAN status checking or health checking. Identify a server predefine by FortiGuard and determine how SD-WAN verifies that FGT can communicate with it. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: health_check_fortiguard:target_name</span>
 <a id='label170' href="javascript:ContentClick('label171', 'label170');" onmouseover="ContentPreview('label171');" onmouseout="ContentUnpreview('label171');" title="click to collapse or expand..."> more... </a>
 <div id="label171" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>health_check_fortiguard</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">addr_mode</span> - Address mode (IPv4 or IPv6). <span class="li-normal">type: str</span> <span class="li-normal">choices: ipv4, ipv6</span>
 <a id='label172' href="javascript:ContentClick('label173', 'label172');" onmouseover="ContentPreview('label173');" onmouseout="ContentUnpreview('label173');" title="click to collapse or expand..."> more... </a>
 <div id="label173" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>addr_mode</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[ipv4]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[ipv6]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">class_id</span> - Traffic class ID. Source firewall.traffic-class.class-id. <span class="li-normal">type: int</span>
 <a id='label174' href="javascript:ContentClick('label175', 'label174');" onmouseover="ContentPreview('label175');" onmouseout="ContentUnpreview('label175');" title="click to collapse or expand..."> more... </a>
 <div id="label175" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>class_id</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">detect_mode</span> - The mode determining how to detect the server. <span class="li-normal">type: str</span> <span class="li-normal">choices: active, passive, prefer-passive, remote, agent-based</span>
 <a id='label176' href="javascript:ContentClick('label177', 'label176');" onmouseover="ContentPreview('label177');" onmouseout="ContentUnpreview('label177');" title="click to collapse or expand..."> more... </a>
 <div id="label177" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>detect_mode</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[active]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[passive]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[prefer-passive]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[remote]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[agent-based]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">diffservcode</span> - Differentiated services code point (DSCP) in the IP header of the probe packet. <span class="li-normal">type: str</span>
 <a id='label178' href="javascript:ContentClick('label179', 'label178');" onmouseover="ContentPreview('label179');" onmouseout="ContentUnpreview('label179');" title="click to collapse or expand..."> more... </a>
 <div id="label179" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>diffservcode</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">dns_match_ip</span> - Response IP expected from DNS server if the protocol is DNS. <span class="li-normal">type: str</span>
 <a id='label180' href="javascript:ContentClick('label181', 'label180');" onmouseover="ContentPreview('label181');" onmouseout="ContentUnpreview('label181');" title="click to collapse or expand..."> more... </a>
 <div id="label181" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dns_match_ip</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">dns_request_domain</span> - Fully qualified domain name to resolve for the DNS probe. <span class="li-normal">type: str</span>
 <a id='label182' href="javascript:ContentClick('label183', 'label182');" onmouseover="ContentPreview('label183');" onmouseout="ContentUnpreview('label183');" title="click to collapse or expand..."> more... </a>
 <div id="label183" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dns_request_domain</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">embed_measured_health</span> - Enable/disable embedding measured health information. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label184' href="javascript:ContentClick('label185', 'label184');" onmouseover="ContentPreview('label185');" onmouseout="ContentUnpreview('label185');" title="click to collapse or expand..."> more... </a>
 <div id="label185" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>embed_measured_health</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">failtime</span> - Number of failures before server is considered lost (1 - 3600). <span class="li-normal">type: int</span>
 <a id='label186' href="javascript:ContentClick('label187', 'label186');" onmouseover="ContentPreview('label187');" onmouseout="ContentUnpreview('label187');" title="click to collapse or expand..."> more... </a>
 <div id="label187" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>failtime</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ftp_file</span> - Full path and file name on the FTP server to download for FTP health-check to probe. <span class="li-normal">type: str</span>
 <a id='label188' href="javascript:ContentClick('label189', 'label188');" onmouseover="ContentPreview('label189');" onmouseout="ContentUnpreview('label189');" title="click to collapse or expand..."> more... </a>
 <div id="label189" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ftp_file</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ftp_mode</span> - FTP mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: passive, port</span>
 <a id='label190' href="javascript:ContentClick('label191', 'label190');" onmouseover="ContentPreview('label191');" onmouseout="ContentUnpreview('label191');" title="click to collapse or expand..."> more... </a>
 <div id="label191" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ftp_mode</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[passive]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[port]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ha_priority</span> - HA election priority (1 - 50). <span class="li-normal">type: int</span>
 <a id='label192' href="javascript:ContentClick('label193', 'label192');" onmouseover="ContentPreview('label193');" onmouseout="ContentUnpreview('label193');" title="click to collapse or expand..."> more... </a>
 <div id="label193" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ha_priority</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">http_agent</span> - String in the http-agent field in the HTTP header. <span class="li-normal">type: str</span>
 <a id='label194' href="javascript:ContentClick('label195', 'label194');" onmouseover="ContentPreview('label195');" onmouseout="ContentUnpreview('label195');" title="click to collapse or expand..."> more... </a>
 <div id="label195" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>http_agent</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">http_get</span> - URL used to communicate with the server if the protocol if the protocol is HTTP. <span class="li-normal">type: str</span>
 <a id='label196' href="javascript:ContentClick('label197', 'label196');" onmouseover="ContentPreview('label197');" onmouseout="ContentUnpreview('label197');" title="click to collapse or expand..."> more... </a>
 <div id="label197" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>http_get</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">http_match</span> - Response string expected from the server if the protocol is HTTP. <span class="li-normal">type: str</span>
 <a id='label198' href="javascript:ContentClick('label199', 'label198');" onmouseover="ContentPreview('label199');" onmouseout="ContentUnpreview('label199');" title="click to collapse or expand..."> more... </a>
 <div id="label199" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>http_match</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">interval</span> - Status check interval in milliseconds, or the time between attempting to connect to the server (20 - 3600*1000 msec). <span class="li-normal">type: int</span>
 <a id='label200' href="javascript:ContentClick('label201', 'label200');" onmouseover="ContentPreview('label201');" onmouseout="ContentUnpreview('label201');" title="click to collapse or expand..."> more... </a>
 <div id="label201" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>interval</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">members</span> - Member sequence number list. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: health_check_fortiguard:target_name/members:seq_num</span>
 <a id='label202' href="javascript:ContentClick('label203', 'label202');" onmouseover="ContentPreview('label203');" onmouseout="ContentUnpreview('label203');" title="click to collapse or expand..."> more... </a>
 <div id="label203" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>members</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">seq_num</span> - Member sequence number. see <a href='#notes'>Notes</a>. Source system.sdwan.members.seq-num. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label204' href="javascript:ContentClick('label205', 'label204');" onmouseover="ContentPreview('label205');" onmouseout="ContentUnpreview('label205');" title="click to collapse or expand..."> more... </a>
 <div id="label205" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>seq_num</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">mos_codec</span> - Codec to use for MOS calculation . <span class="li-normal">type: str</span> <span class="li-normal">choices: g711, g722, g729</span>
 <a id='label206' href="javascript:ContentClick('label207', 'label206');" onmouseover="ContentPreview('label207');" onmouseout="ContentUnpreview('label207');" title="click to collapse or expand..."> more... </a>
 <div id="label207" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mos_codec</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[g711]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[g722]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[g729]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">packet_size</span> - Packet size of a TWAMP test session. (124/158 - 1024) <span class="li-normal">type: int</span>
 <a id='label208' href="javascript:ContentClick('label209', 'label208');" onmouseover="ContentPreview('label209');" onmouseout="ContentUnpreview('label209');" title="click to collapse or expand..."> more... </a>
 <div id="label209" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>packet_size</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">password</span> - TWAMP controller password in authentication mode. <span class="li-normal">type: str</span>
 <a id='label210' href="javascript:ContentClick('label211', 'label210');" onmouseover="ContentPreview('label211');" onmouseout="ContentUnpreview('label211');" title="click to collapse or expand..."> more... </a>
 <div id="label211" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>password</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">port</span> - Port number used to communicate with the server over the selected protocol (0 - 65535). <span class="li-normal">type: int</span>
 <a id='label212' href="javascript:ContentClick('label213', 'label212');" onmouseover="ContentPreview('label213');" onmouseout="ContentUnpreview('label213');" title="click to collapse or expand..."> more... </a>
 <div id="label213" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>port</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">probe_count</span> - Number of most recent probes that should be used to calculate latency and jitter (5 - 30). <span class="li-normal">type: int</span>
 <a id='label214' href="javascript:ContentClick('label215', 'label214');" onmouseover="ContentPreview('label215');" onmouseout="ContentUnpreview('label215');" title="click to collapse or expand..."> more... </a>
 <div id="label215" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>probe_count</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">probe_packets</span> - Enable/disable transmission of probe packets. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label216' href="javascript:ContentClick('label217', 'label216');" onmouseover="ContentPreview('label217');" onmouseout="ContentUnpreview('label217');" title="click to collapse or expand..."> more... </a>
 <div id="label217" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>probe_packets</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">probe_timeout</span> - Time to wait before a probe packet is considered lost (20 - 3600*1000 msec). <span class="li-normal">type: int</span>
 <a id='label218' href="javascript:ContentClick('label219', 'label218');" onmouseover="ContentPreview('label219');" onmouseout="ContentUnpreview('label219');" title="click to collapse or expand..."> more... </a>
 <div id="label219" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>probe_timeout</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">protocol</span> - Protocol used to determine if the FortiGate can communicate with the server. <span class="li-normal">type: str</span> <span class="li-normal">choices: ping, tcp-echo, udp-echo, http, https, twamp, dns, tcp-connect, ftp</span>
 <a id='label220' href="javascript:ContentClick('label221', 'label220');" onmouseover="ContentPreview('label221');" onmouseout="ContentUnpreview('label221');" title="click to collapse or expand..."> more... </a>
 <div id="label221" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>protocol</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[ping]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[tcp-echo]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[udp-echo]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[http]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[https]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[twamp]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[dns]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[tcp-connect]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[ftp]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">quality_measured_method</span> - Method to measure the quality of tcp-connect. <span class="li-normal">type: str</span> <span class="li-normal">choices: half-open, half-close</span>
 <a id='label222' href="javascript:ContentClick('label223', 'label222');" onmouseover="ContentPreview('label223');" onmouseout="ContentUnpreview('label223');" title="click to collapse or expand..."> more... </a>
 <div id="label223" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>quality_measured_method</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[half-open]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[half-close]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">recoverytime</span> - Number of successful responses received before server is considered recovered (1 - 3600). <span class="li-normal">type: int</span>
 <a id='label224' href="javascript:ContentClick('label225', 'label224');" onmouseover="ContentPreview('label225');" onmouseout="ContentUnpreview('label225');" title="click to collapse or expand..."> more... </a>
 <div id="label225" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>recoverytime</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">security_mode</span> - Twamp controller security mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, authentication</span>
 <a id='label226' href="javascript:ContentClick('label227', 'label226');" onmouseover="ContentPreview('label227');" onmouseout="ContentUnpreview('label227');" title="click to collapse or expand..."> more... </a>
 <div id="label227" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>security_mode</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[authentication]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">server</span> - Predefined IP address or FQDN name from FortiGuard. <span class="li-normal">type: list</span> </li>
            <li> <span class="li-head">sla</span> - Service level agreement (SLA). <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: health_check_fortiguard:target_name/sla:id</span>
 <a id='label228' href="javascript:ContentClick('label229', 'label228');" onmouseover="ContentPreview('label229');" onmouseout="ContentUnpreview('label229');" title="click to collapse or expand..."> more... </a>
 <div id="label229" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sla</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">id</span> - SLA ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label230' href="javascript:ContentClick('label231', 'label230');" onmouseover="ContentPreview('label231');" onmouseout="ContentUnpreview('label231');" title="click to collapse or expand..."> more... </a>
 <div id="label231" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">jitter_threshold</span> - Jitter for SLA to make decision in milliseconds. (0 - 10000000). <span class="li-normal">type: int</span>
 <a id='label232' href="javascript:ContentClick('label233', 'label232');" onmouseover="ContentPreview('label233');" onmouseout="ContentUnpreview('label233');" title="click to collapse or expand..."> more... </a>
 <div id="label233" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>jitter_threshold</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">latency_threshold</span> - Latency for SLA to make decision in milliseconds. (0 - 10000000). <span class="li-normal">type: int</span>
 <a id='label234' href="javascript:ContentClick('label235', 'label234');" onmouseover="ContentPreview('label235');" onmouseout="ContentUnpreview('label235');" title="click to collapse or expand..."> more... </a>
 <div id="label235" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>latency_threshold</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">link_cost_factor</span> - Criteria on which to base link selection. <span class="li-normal">type: list</span> <span class="li-normal">choices: latency, jitter, packet-loss, mos, remote</span>
 <a id='label236' href="javascript:ContentClick('label237', 'label236');" onmouseover="ContentPreview('label237');" onmouseout="ContentUnpreview('label237');" title="click to collapse or expand..."> more... </a>
 <div id="label237" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>link_cost_factor</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[latency]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[jitter]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[packet-loss]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[mos]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[remote]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">mos_threshold</span> - Minimum Mean Opinion Score for SLA to be marked as pass. (1.0 - 5.0). <span class="li-normal">type: str</span>
 <a id='label238' href="javascript:ContentClick('label239', 'label238');" onmouseover="ContentPreview('label239');" onmouseout="ContentUnpreview('label239');" title="click to collapse or expand..."> more... </a>
 <div id="label239" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mos_threshold</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">packetloss_threshold</span> - Packet loss for SLA to make decision in percentage. (0 - 100). <span class="li-normal">type: int</span>
 <a id='label240' href="javascript:ContentClick('label241', 'label240');" onmouseover="ContentPreview('label241');" onmouseout="ContentUnpreview('label241');" title="click to collapse or expand..."> more... </a>
 <div id="label241" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>packetloss_threshold</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">priority_in_sla</span> - Value to be distributed into routing table when in-sla (0 - 65535). <span class="li-normal">type: int</span>
 <a id='label242' href="javascript:ContentClick('label243', 'label242');" onmouseover="ContentPreview('label243');" onmouseout="ContentUnpreview('label243');" title="click to collapse or expand..."> more... </a>
 <div id="label243" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>priority_in_sla</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">priority_out_sla</span> - Value to be distributed into routing table when out-sla (0 - 65535). <span class="li-normal">type: int</span>
 <a id='label244' href="javascript:ContentClick('label245', 'label244');" onmouseover="ContentPreview('label245');" onmouseout="ContentUnpreview('label245');" title="click to collapse or expand..."> more... </a>
 <div id="label245" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>priority_out_sla</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">sla_fail_log_period</span> - Time interval in seconds that SLA fail log messages will be generated (0 - 3600). <span class="li-normal">type: int</span>
 <a id='label246' href="javascript:ContentClick('label247', 'label246');" onmouseover="ContentPreview('label247');" onmouseout="ContentUnpreview('label247');" title="click to collapse or expand..."> more... </a>
 <div id="label247" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sla_fail_log_period</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">sla_id_redistribute</span> - Select the ID from the SLA sub-table. The selected SLA"s priority value will be distributed into the routing table (0 - 32). <span class="li-normal">type: int</span>
 <a id='label248' href="javascript:ContentClick('label249', 'label248');" onmouseover="ContentPreview('label249');" onmouseout="ContentUnpreview('label249');" title="click to collapse or expand..."> more... </a>
 <div id="label249" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sla_id_redistribute</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">sla_pass_log_period</span> - Time interval in seconds that SLA pass log messages will be generated (0 - 3600). <span class="li-normal">type: int</span>
 <a id='label250' href="javascript:ContentClick('label251', 'label250');" onmouseover="ContentPreview('label251');" onmouseout="ContentUnpreview('label251');" title="click to collapse or expand..."> more... </a>
 <div id="label251" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sla_pass_log_period</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">source</span> - Source IP address used in the health-check packet to the server. <span class="li-normal">type: str</span>
 <a id='label252' href="javascript:ContentClick('label253', 'label252');" onmouseover="ContentPreview('label253');" onmouseout="ContentUnpreview('label253');" title="click to collapse or expand..."> more... </a>
 <div id="label253" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>source</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">source6</span> - Source IPv6 address used in the health-check packet to server. <span class="li-normal">type: str</span>
 <a id='label254' href="javascript:ContentClick('label255', 'label254');" onmouseover="ContentPreview('label255');" onmouseout="ContentUnpreview('label255');" title="click to collapse or expand..."> more... </a>
 <div id="label255" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>source6</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">system_dns</span> - Enable/disable system DNS as the probe server. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label256' href="javascript:ContentClick('label257', 'label256');" onmouseover="ContentPreview('label257');" onmouseout="ContentUnpreview('label257');" title="click to collapse or expand..."> more... </a>
 <div id="label257" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>system_dns</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">target_name</span> - Status check or predefined health-check targets name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label258' href="javascript:ContentClick('label259', 'label258');" onmouseover="ContentPreview('label259');" onmouseout="ContentUnpreview('label259');" title="click to collapse or expand..."> more... </a>
 <div id="label259" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>target_name</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">threshold_alert_jitter</span> - Alert threshold for jitter (ms). <span class="li-normal">type: int</span>
 <a id='label260' href="javascript:ContentClick('label261', 'label260');" onmouseover="ContentPreview('label261');" onmouseout="ContentUnpreview('label261');" title="click to collapse or expand..."> more... </a>
 <div id="label261" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>threshold_alert_jitter</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">threshold_alert_latency</span> - Alert threshold for latency (ms). <span class="li-normal">type: int</span>
 <a id='label262' href="javascript:ContentClick('label263', 'label262');" onmouseover="ContentPreview('label263');" onmouseout="ContentUnpreview('label263');" title="click to collapse or expand..."> more... </a>
 <div id="label263" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>threshold_alert_latency</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">threshold_alert_packetloss</span> - Alert threshold for packet loss (percentage). <span class="li-normal">type: int</span>
 <a id='label264' href="javascript:ContentClick('label265', 'label264');" onmouseover="ContentPreview('label265');" onmouseout="ContentUnpreview('label265');" title="click to collapse or expand..."> more... </a>
 <div id="label265" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>threshold_alert_packetloss</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">threshold_warning_jitter</span> - Warning threshold for jitter (ms). <span class="li-normal">type: int</span>
 <a id='label266' href="javascript:ContentClick('label267', 'label266');" onmouseover="ContentPreview('label267');" onmouseout="ContentUnpreview('label267');" title="click to collapse or expand..."> more... </a>
 <div id="label267" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>threshold_warning_jitter</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">threshold_warning_latency</span> - Warning threshold for latency (ms). <span class="li-normal">type: int</span>
 <a id='label268' href="javascript:ContentClick('label269', 'label268');" onmouseover="ContentPreview('label269');" onmouseout="ContentUnpreview('label269');" title="click to collapse or expand..."> more... </a>
 <div id="label269" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>threshold_warning_latency</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">threshold_warning_packetloss</span> - Warning threshold for packet loss (percentage). <span class="li-normal">type: int</span>
 <a id='label270' href="javascript:ContentClick('label271', 'label270');" onmouseover="ContentPreview('label271');" onmouseout="ContentUnpreview('label271');" title="click to collapse or expand..."> more... </a>
 <div id="label271" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>threshold_warning_packetloss</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">update_cascade_interface</span> - Enable/disable update cascade interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label272' href="javascript:ContentClick('label273', 'label272');" onmouseover="ContentPreview('label273');" onmouseout="ContentUnpreview('label273');" title="click to collapse or expand..."> more... </a>
 <div id="label273" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>update_cascade_interface</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">update_static_route</span> - Enable/disable updating the static route. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label274' href="javascript:ContentClick('label275', 'label274');" onmouseover="ContentPreview('label275');" onmouseout="ContentUnpreview('label275');" title="click to collapse or expand..."> more... </a>
 <div id="label275" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>update_static_route</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">user</span> - The user name to access probe server. <span class="li-normal">type: str</span>
 <a id='label276' href="javascript:ContentClick('label277', 'label276');" onmouseover="ContentPreview('label277');" onmouseout="ContentUnpreview('label277');" title="click to collapse or expand..."> more... </a>
 <div id="label277" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>user</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">vrf</span> - Virtual Routing Forwarding ID. <span class="li-normal">type: int</span>
 <a id='label278' href="javascript:ContentClick('label279', 'label278');" onmouseover="ContentPreview('label279');" onmouseout="ContentUnpreview('label279');" title="click to collapse or expand..."> more... </a>
 <div id="label279" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vrf</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">load_balance_mode</span> - Algorithm or mode to use for load balancing Internet traffic to SD-WAN members. <span class="li-normal">type: str</span> <span class="li-normal">choices: source-ip-based, weight-based, usage-based, source-dest-ip-based, measured-volume-based</span>
 <a id='label280' href="javascript:ContentClick('label281', 'label280');" onmouseover="ContentPreview('label281');" onmouseout="ContentUnpreview('label281');" title="click to collapse or expand..."> more... </a>
 <div id="label281" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>load_balance_mode</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[source-ip-based]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[weight-based]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[usage-based]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[source-dest-ip-based]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[measured-volume-based]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">members</span> - FortiGate interfaces added to the SD-WAN. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: members:seq_num</span>
 <a id='label282' href="javascript:ContentClick('label283', 'label282');" onmouseover="ContentPreview('label283');" onmouseout="ContentUnpreview('label283');" title="click to collapse or expand..."> more... </a>
 <div id="label283" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>members</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">comment</span> - Comments. <span class="li-normal">type: str</span>
 <a id='label284' href="javascript:ContentClick('label285', 'label284');" onmouseover="ContentPreview('label285');" onmouseout="ContentUnpreview('label285');" title="click to collapse or expand..."> more... </a>
 <div id="label285" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>comment</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">cost</span> - Cost of this interface for services in SLA mode (0 - 4294967295). <span class="li-normal">type: int</span>
 <a id='label286' href="javascript:ContentClick('label287', 'label286');" onmouseover="ContentPreview('label287');" onmouseout="ContentUnpreview('label287');" title="click to collapse or expand..."> more... </a>
 <div id="label287" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cost</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">gateway</span> - The default gateway for this interface. Usually the default gateway of the Internet service provider that this interface is connected to. <span class="li-normal">type: str</span>
 <a id='label288' href="javascript:ContentClick('label289', 'label288');" onmouseover="ContentPreview('label289');" onmouseout="ContentUnpreview('label289');" title="click to collapse or expand..."> more... </a>
 <div id="label289" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gateway</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">gateway6</span> - IPv6 gateway. <span class="li-normal">type: str</span>
 <a id='label290' href="javascript:ContentClick('label291', 'label290');" onmouseover="ContentPreview('label291');" onmouseout="ContentUnpreview('label291');" title="click to collapse or expand..."> more... </a>
 <div id="label291" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gateway6</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ingress_spillover_threshold</span> - Ingress spillover threshold for this interface (0 - 16776000 kbit/s). When this traffic volume threshold is reached, new sessions spill over to other interfaces in the SD-WAN. <span class="li-normal">type: int</span>
 <a id='label292' href="javascript:ContentClick('label293', 'label292');" onmouseover="ContentPreview('label293');" onmouseout="ContentUnpreview('label293');" title="click to collapse or expand..."> more... </a>
 <div id="label293" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ingress_spillover_threshold</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">interface</span> - Interface name. Source system.interface.name. <span class="li-normal">type: str</span>
 <a id='label294' href="javascript:ContentClick('label295', 'label294');" onmouseover="ContentPreview('label295');" onmouseout="ContentUnpreview('label295');" title="click to collapse or expand..."> more... </a>
 <div id="label295" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>interface</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">preferred_source</span> - Preferred source of route for this member. <span class="li-normal">type: str</span>
 <a id='label296' href="javascript:ContentClick('label297', 'label296');" onmouseover="ContentPreview('label297');" onmouseout="ContentUnpreview('label297');" title="click to collapse or expand..."> more... </a>
 <div id="label297" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>preferred_source</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">priority</span> - Priority of the interface for IPv4 (1 - 65535). Used for SD-WAN rules or priority rules. <span class="li-normal">type: int</span>
 <a id='label298' href="javascript:ContentClick('label299', 'label298');" onmouseover="ContentPreview('label299');" onmouseout="ContentUnpreview('label299');" title="click to collapse or expand..."> more... </a>
 <div id="label299" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>priority</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">priority_in_sla</span> - Preferred priority of routes to this member when this member is in-sla (0 - 65535). <span class="li-normal">type: int</span>
 <a id='label300' href="javascript:ContentClick('label301', 'label300');" onmouseover="ContentPreview('label301');" onmouseout="ContentUnpreview('label301');" title="click to collapse or expand..."> more... </a>
 <div id="label301" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>priority_in_sla</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">priority_out_sla</span> - Preferred priority of routes to this member when this member is out-of-sla (0 - 65535). <span class="li-normal">type: int</span>
 <a id='label302' href="javascript:ContentClick('label303', 'label302');" onmouseover="ContentPreview('label303');" onmouseout="ContentUnpreview('label303');" title="click to collapse or expand..."> more... </a>
 <div id="label303" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>priority_out_sla</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">priority6</span> - Priority of the interface for IPv6 (1 - 65535). Used for SD-WAN rules or priority rules. <span class="li-normal">type: int</span>
 <a id='label304' href="javascript:ContentClick('label305', 'label304');" onmouseover="ContentPreview('label305');" onmouseout="ContentUnpreview('label305');" title="click to collapse or expand..."> more... </a>
 <div id="label305" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>priority6</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">seq_num</span> - Sequence number(1-512). see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label306' href="javascript:ContentClick('label307', 'label306');" onmouseover="ContentPreview('label307');" onmouseout="ContentUnpreview('label307');" title="click to collapse or expand..."> more... </a>
 <div id="label307" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>seq_num</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">source</span> - Source IP address used in the health-check packet to the server. <span class="li-normal">type: str</span>
 <a id='label308' href="javascript:ContentClick('label309', 'label308');" onmouseover="ContentPreview('label309');" onmouseout="ContentUnpreview('label309');" title="click to collapse or expand..."> more... </a>
 <div id="label309" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>source</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">source6</span> - Source IPv6 address used in the health-check packet to the server. <span class="li-normal">type: str</span>
 <a id='label310' href="javascript:ContentClick('label311', 'label310');" onmouseover="ContentPreview('label311');" onmouseout="ContentUnpreview('label311');" title="click to collapse or expand..."> more... </a>
 <div id="label311" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>source6</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">spillover_threshold</span> - Egress spillover threshold for this interface (0 - 16776000 kbit/s). When this traffic volume threshold is reached, new sessions spill over to other interfaces in the SD-WAN. <span class="li-normal">type: int</span>
 <a id='label312' href="javascript:ContentClick('label313', 'label312');" onmouseover="ContentPreview('label313');" onmouseout="ContentUnpreview('label313');" title="click to collapse or expand..."> more... </a>
 <div id="label313" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>spillover_threshold</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">status</span> - Enable/disable this interface in the SD-WAN. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label314' href="javascript:ContentClick('label315', 'label314');" onmouseover="ContentPreview('label315');" onmouseout="ContentUnpreview('label315');" title="click to collapse or expand..."> more... </a>
 <div id="label315" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">transport_group</span> - Measured transport group (0 - 255). <span class="li-normal">type: int</span>
 <a id='label316' href="javascript:ContentClick('label317', 'label316');" onmouseover="ContentPreview('label317');" onmouseout="ContentUnpreview('label317');" title="click to collapse or expand..."> more... </a>
 <div id="label317" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>transport_group</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">volume_ratio</span> - Measured volume ratio (this value / sum of all values = percentage of link volume, 1 - 255). <span class="li-normal">type: int</span>
 <a id='label318' href="javascript:ContentClick('label319', 'label318');" onmouseover="ContentPreview('label319');" onmouseout="ContentUnpreview('label319');" title="click to collapse or expand..."> more... </a>
 <div id="label319" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>volume_ratio</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">weight</span> - Weight of this interface for weighted load balancing. (1 - 255) More traffic is directed to interfaces with higher weights. <span class="li-normal">type: int</span>
 <a id='label320' href="javascript:ContentClick('label321', 'label320');" onmouseover="ContentPreview('label321');" onmouseout="ContentUnpreview('label321');" title="click to collapse or expand..."> more... </a>
 <div id="label321" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>weight</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">zone</span> - Zone name. Source system.sdwan.zone.name. <span class="li-normal">type: str</span>
 <a id='label322' href="javascript:ContentClick('label323', 'label322');" onmouseover="ContentPreview('label323');" onmouseout="ContentUnpreview('label323');" title="click to collapse or expand..."> more... </a>
 <div id="label323" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>zone</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">neighbor</span> - Create SD-WAN neighbor from BGP neighbor table to control route advertisements according to SLA status. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: neighbor:ip</span>
 <a id='label324' href="javascript:ContentClick('label325', 'label324');" onmouseover="ContentPreview('label325');" onmouseout="ContentUnpreview('label325');" title="click to collapse or expand..."> more... </a>
 <div id="label325" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>neighbor</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">health_check</span> - SD-WAN health-check name. Source system.sdwan.health-check.name. <span class="li-normal">type: str</span>
 <a id='label326' href="javascript:ContentClick('label327', 'label326');" onmouseover="ContentPreview('label327');" onmouseout="ContentUnpreview('label327');" title="click to collapse or expand..."> more... </a>
 <div id="label327" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>health_check</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ip</span> - IP/IPv6 address of neighbor or neighbor-group name. Source router.bgp.neighbor-group.name router.bgp.neighbor.ip. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label328' href="javascript:ContentClick('label329', 'label328');" onmouseover="ContentPreview('label329');" onmouseout="ContentUnpreview('label329');" title="click to collapse or expand..."> more... </a>
 <div id="label329" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ip</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">member</span> - Member sequence number list. Source system.sdwan.members.seq-num. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: neighbor:ip/member:seq_num</span>
 <a id='label330' href="javascript:ContentClick('label331', 'label330');" onmouseover="ContentPreview('label331');" onmouseout="ContentUnpreview('label331');" title="click to collapse or expand..."> more... </a>
 <div id="label331" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>member</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">seq_num</span> - Member sequence number. see <a href='#notes'>Notes</a>. Source system.sdwan.members.seq-num. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label332' href="javascript:ContentClick('label333', 'label332');" onmouseover="ContentPreview('label333');" onmouseout="ContentUnpreview('label333');" title="click to collapse or expand..."> more... </a>
 <div id="label333" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>seq_num</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">minimum_sla_meet_members</span> - Minimum number of members which meet SLA when the neighbor is preferred. <span class="li-normal">type: int</span>
 <a id='label334' href="javascript:ContentClick('label335', 'label334');" onmouseover="ContentPreview('label335');" onmouseout="ContentUnpreview('label335');" title="click to collapse or expand..."> more... </a>
 <div id="label335" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>minimum_sla_meet_members</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mode</span> - What metric to select the neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: sla, speedtest</span>
 <a id='label336' href="javascript:ContentClick('label337', 'label336');" onmouseover="ContentPreview('label337');" onmouseout="ContentUnpreview('label337');" title="click to collapse or expand..."> more... </a>
 <div id="label337" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mode</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[sla]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[speedtest]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">role</span> - Role of neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: standalone, primary, secondary</span>
 <a id='label338' href="javascript:ContentClick('label339', 'label338');" onmouseover="ContentPreview('label339');" onmouseout="ContentUnpreview('label339');" title="click to collapse or expand..."> more... </a>
 <div id="label339" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>role</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[standalone]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[primary]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[secondary]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">route_metric</span> - Route-metric of neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: preferable, priority</span>
 <a id='label340' href="javascript:ContentClick('label341', 'label340');" onmouseover="ContentPreview('label341');" onmouseout="ContentUnpreview('label341');" title="click to collapse or expand..."> more... </a>
 <div id="label341" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>route_metric</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[preferable]</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.2</code></td>
 <tr>
 <td>[priority]</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">service_id</span> - SD-WAN service ID to work with the neighbor. Source system.sdwan.service.id. <span class="li-normal">type: int</span>
 <a id='label342' href="javascript:ContentClick('label343', 'label342');" onmouseover="ContentPreview('label343');" onmouseout="ContentUnpreview('label343');" title="click to collapse or expand..."> more... </a>
 <div id="label343" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>service_id</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">sla_id</span> - SLA ID. <span class="li-normal">type: int</span>
 <a id='label344' href="javascript:ContentClick('label345', 'label344');" onmouseover="ContentPreview('label345');" onmouseout="ContentUnpreview('label345');" title="click to collapse or expand..."> more... </a>
 <div id="label345" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sla_id</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">neighbor_hold_boot_time</span> - Waiting period in seconds when switching from the primary neighbor to the secondary neighbor from the neighbor start. (0 - 10000000). <span class="li-normal">type: int</span>
 <a id='label346' href="javascript:ContentClick('label347', 'label346');" onmouseover="ContentPreview('label347');" onmouseout="ContentUnpreview('label347');" title="click to collapse or expand..."> more... </a>
 <div id="label347" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>neighbor_hold_boot_time</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">neighbor_hold_down</span> - Enable/disable hold switching from the secondary neighbor to the primary neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label348' href="javascript:ContentClick('label349', 'label348');" onmouseover="ContentPreview('label349');" onmouseout="ContentUnpreview('label349');" title="click to collapse or expand..."> more... </a>
 <div id="label349" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>neighbor_hold_down</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">neighbor_hold_down_time</span> - Waiting period in seconds when switching from the secondary neighbor to the primary neighbor when hold-down is disabled. (0 - 10000000). <span class="li-normal">type: int</span>
 <a id='label350' href="javascript:ContentClick('label351', 'label350');" onmouseover="ContentPreview('label351');" onmouseout="ContentUnpreview('label351');" title="click to collapse or expand..."> more... </a>
 <div id="label351" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>neighbor_hold_down_time</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">service</span> - Create SD-WAN rules (also called services) to control how sessions are distributed to interfaces in the SD-WAN. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: service:id</span>
 <a id='label352' href="javascript:ContentClick('label353', 'label352');" onmouseover="ContentPreview('label353');" onmouseout="ContentUnpreview('label353');" title="click to collapse or expand..."> more... </a>
 <div id="label353" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>service</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">addr_mode</span> - Address mode (IPv4 or IPv6). <span class="li-normal">type: str</span> <span class="li-normal">choices: ipv4, ipv6</span>
 <a id='label354' href="javascript:ContentClick('label355', 'label354');" onmouseover="ContentPreview('label355');" onmouseout="ContentUnpreview('label355');" title="click to collapse or expand..."> more... </a>
 <div id="label355" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>addr_mode</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[ipv4]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[ipv6]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">agent_exclusive</span> - Set/unset the service as agent use exclusively. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label356' href="javascript:ContentClick('label357', 'label356');" onmouseover="ContentPreview('label357');" onmouseout="ContentUnpreview('label357');" title="click to collapse or expand..."> more... </a>
 <div id="label357" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>agent_exclusive</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">bandwidth_weight</span> - Coefficient of reciprocal of available bidirectional bandwidth in the formula of custom-profile-1. <span class="li-normal">type: int</span>
 <a id='label358' href="javascript:ContentClick('label359', 'label358');" onmouseover="ContentPreview('label359');" onmouseout="ContentUnpreview('label359');" title="click to collapse or expand..."> more... </a>
 <div id="label359" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>bandwidth_weight</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">comment</span> - Comments. <span class="li-normal">type: str</span>
 <a id='label360' href="javascript:ContentClick('label361', 'label360');" onmouseover="ContentPreview('label361');" onmouseout="ContentUnpreview('label361');" title="click to collapse or expand..."> more... </a>
 <div id="label361" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>comment</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">default</span> - Enable/disable use of SD-WAN as default service. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label362' href="javascript:ContentClick('label363', 'label362');" onmouseover="ContentPreview('label363');" onmouseout="ContentUnpreview('label363');" title="click to collapse or expand..."> more... </a>
 <div id="label363" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>default</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">dscp_forward</span> - Enable/disable forward traffic DSCP tag. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label364' href="javascript:ContentClick('label365', 'label364');" onmouseover="ContentPreview('label365');" onmouseout="ContentUnpreview('label365');" title="click to collapse or expand..."> more... </a>
 <div id="label365" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp_forward</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">dscp_forward_tag</span> - Forward traffic DSCP tag. <span class="li-normal">type: str</span>
 <a id='label366' href="javascript:ContentClick('label367', 'label366');" onmouseover="ContentPreview('label367');" onmouseout="ContentUnpreview('label367');" title="click to collapse or expand..."> more... </a>
 <div id="label367" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp_forward_tag</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">dscp_reverse</span> - Enable/disable reverse traffic DSCP tag. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label368' href="javascript:ContentClick('label369', 'label368');" onmouseover="ContentPreview('label369');" onmouseout="ContentUnpreview('label369');" title="click to collapse or expand..."> more... </a>
 <div id="label369" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp_reverse</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">dscp_reverse_tag</span> - Reverse traffic DSCP tag. <span class="li-normal">type: str</span>
 <a id='label370' href="javascript:ContentClick('label371', 'label370');" onmouseover="ContentPreview('label371');" onmouseout="ContentUnpreview('label371');" title="click to collapse or expand..."> more... </a>
 <div id="label371" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp_reverse_tag</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">dst</span> - Destination address name. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: service:id/dst:name</span>
 <a id='label372' href="javascript:ContentClick('label373', 'label372');" onmouseover="ContentPreview('label373');" onmouseout="ContentUnpreview('label373');" title="click to collapse or expand..."> more... </a>
 <div id="label373" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dst</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Address or address group name. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label374' href="javascript:ContentClick('label375', 'label374');" onmouseover="ContentPreview('label375');" onmouseout="ContentUnpreview('label375');" title="click to collapse or expand..."> more... </a>
 <div id="label375" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">dst_negate</span> - Enable/disable negation of destination address match. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label376' href="javascript:ContentClick('label377', 'label376');" onmouseover="ContentPreview('label377');" onmouseout="ContentUnpreview('label377');" title="click to collapse or expand..."> more... </a>
 <div id="label377" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dst_negate</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">dst6</span> - Destination address6 name. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: service:id/dst6:name</span>
 <a id='label378' href="javascript:ContentClick('label379', 'label378');" onmouseover="ContentPreview('label379');" onmouseout="ContentUnpreview('label379');" title="click to collapse or expand..."> more... </a>
 <div id="label379" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dst6</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Address6 or address6 group name. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label380' href="javascript:ContentClick('label381', 'label380');" onmouseover="ContentPreview('label381');" onmouseout="ContentUnpreview('label381');" title="click to collapse or expand..."> more... </a>
 <div id="label381" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">end_port</span> - End destination port number. <span class="li-normal">type: int</span>
 <a id='label382' href="javascript:ContentClick('label383', 'label382');" onmouseover="ContentPreview('label383');" onmouseout="ContentUnpreview('label383');" title="click to collapse or expand..."> more... </a>
 <div id="label383" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>end_port</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">end_src_port</span> - End source port number. <span class="li-normal">type: int</span>
 <a id='label384' href="javascript:ContentClick('label385', 'label384');" onmouseover="ContentPreview('label385');" onmouseout="ContentUnpreview('label385');" title="click to collapse or expand..."> more... </a>
 <div id="label385" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>end_src_port</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">gateway</span> - Enable/disable SD-WAN service gateway. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label386' href="javascript:ContentClick('label387', 'label386');" onmouseover="ContentPreview('label387');" onmouseout="ContentUnpreview('label387');" title="click to collapse or expand..."> more... </a>
 <div id="label387" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gateway</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">groups</span> - User groups. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: service:id/groups:name</span>
 <a id='label388' href="javascript:ContentClick('label389', 'label388');" onmouseover="ContentPreview('label389');" onmouseout="ContentUnpreview('label389');" title="click to collapse or expand..."> more... </a>
 <div id="label389" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>groups</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Group name. Source user.group.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label390' href="javascript:ContentClick('label391', 'label390');" onmouseover="ContentPreview('label391');" onmouseout="ContentUnpreview('label391');" title="click to collapse or expand..."> more... </a>
 <div id="label391" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">hash_mode</span> - Hash algorithm for selected priority members for load balance mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: round-robin, source-ip-based, source-dest-ip-based, inbandwidth, outbandwidth, bibandwidth</span>
 <a id='label392' href="javascript:ContentClick('label393', 'label392');" onmouseover="ContentPreview('label393');" onmouseout="ContentUnpreview('label393');" title="click to collapse or expand..."> more... </a>
 <div id="label393" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>hash_mode</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[round-robin]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <tr>
 <td>[source-ip-based]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <tr>
 <td>[source-dest-ip-based]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <tr>
 <td>[inbandwidth]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <tr>
 <td>[outbandwidth]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <tr>
 <td>[bibandwidth]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">health_check</span> - Health check list. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: service:id/health_check:name</span>
 <a id='label394' href="javascript:ContentClick('label395', 'label394');" onmouseover="ContentPreview('label395');" onmouseout="ContentUnpreview('label395');" title="click to collapse or expand..."> more... </a>
 <div id="label395" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>health_check</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Health check name. Source system.sdwan.health-check.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label396' href="javascript:ContentClick('label397', 'label396');" onmouseover="ContentPreview('label397');" onmouseout="ContentUnpreview('label397');" title="click to collapse or expand..."> more... </a>
 <div id="label397" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">hold_down_time</span> - Waiting period in seconds when switching from the back-up member to the primary member (0 - 10000000). <span class="li-normal">type: int</span>
 <a id='label398' href="javascript:ContentClick('label399', 'label398');" onmouseover="ContentPreview('label399');" onmouseout="ContentUnpreview('label399');" title="click to collapse or expand..."> more... </a>
 <div id="label399" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>hold_down_time</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">id</span> - SD-WAN rule ID (1 - 4000). see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label400' href="javascript:ContentClick('label401', 'label400');" onmouseover="ContentPreview('label401');" onmouseout="ContentUnpreview('label401');" title="click to collapse or expand..."> more... </a>
 <div id="label401" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">input_device</span> - Source interface name. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: service:id/input_device:name</span>
 <a id='label402' href="javascript:ContentClick('label403', 'label402');" onmouseover="ContentPreview('label403');" onmouseout="ContentUnpreview('label403');" title="click to collapse or expand..."> more... </a>
 <div id="label403" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>input_device</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Interface name. Source system.interface.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label404' href="javascript:ContentClick('label405', 'label404');" onmouseover="ContentPreview('label405');" onmouseout="ContentUnpreview('label405');" title="click to collapse or expand..."> more... </a>
 <div id="label405" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">input_device_negate</span> - Enable/disable negation of input device match. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label406' href="javascript:ContentClick('label407', 'label406');" onmouseover="ContentPreview('label407');" onmouseout="ContentUnpreview('label407');" title="click to collapse or expand..."> more... </a>
 <div id="label407" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>input_device_negate</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">input_zone</span> - Source input-zone name. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: service:id/input_zone:name</span>
 <a id='label408' href="javascript:ContentClick('label409', 'label408');" onmouseover="ContentPreview('label409');" onmouseout="ContentUnpreview('label409');" title="click to collapse or expand..."> more... </a>
 <div id="label409" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>input_zone</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Zone. Source system.sdwan.zone.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label410' href="javascript:ContentClick('label411', 'label410');" onmouseover="ContentPreview('label411');" onmouseout="ContentUnpreview('label411');" title="click to collapse or expand..."> more... </a>
 <div id="label411" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">internet_service</span> - Enable/disable use of Internet service for application-based load balancing. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label412' href="javascript:ContentClick('label413', 'label412');" onmouseover="ContentPreview('label413');" onmouseout="ContentUnpreview('label413');" title="click to collapse or expand..."> more... </a>
 <div id="label413" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>internet_service</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">internet_service_app_ctrl</span> - Application control based Internet Service ID list. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: service:id/internet_service_app_ctrl:id</span>
 <a id='label414' href="javascript:ContentClick('label415', 'label414');" onmouseover="ContentPreview('label415');" onmouseout="ContentUnpreview('label415');" title="click to collapse or expand..."> more... </a>
 <div id="label415" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>internet_service_app_ctrl</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">id</span> - Application control based Internet Service ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label416' href="javascript:ContentClick('label417', 'label416');" onmouseover="ContentPreview('label417');" onmouseout="ContentUnpreview('label417');" title="click to collapse or expand..."> more... </a>
 <div id="label417" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">internet_service_app_ctrl_category</span> - IDs of one or more application control categories. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: service:id/internet_service_app_ctrl_category:id</span>
 <a id='label418' href="javascript:ContentClick('label419', 'label418');" onmouseover="ContentPreview('label419');" onmouseout="ContentUnpreview('label419');" title="click to collapse or expand..."> more... </a>
 <div id="label419" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>internet_service_app_ctrl_category</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">id</span> - Application control category ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label420' href="javascript:ContentClick('label421', 'label420');" onmouseover="ContentPreview('label421');" onmouseout="ContentUnpreview('label421');" title="click to collapse or expand..."> more... </a>
 <div id="label421" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">internet_service_app_ctrl_group</span> - Application control based Internet Service group list. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: service:id/internet_service_app_ctrl_group:name</span>
 <a id='label422' href="javascript:ContentClick('label423', 'label422');" onmouseover="ContentPreview('label423');" onmouseout="ContentUnpreview('label423');" title="click to collapse or expand..."> more... </a>
 <div id="label423" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>internet_service_app_ctrl_group</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Application control based Internet Service group name. Source application.group.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label424' href="javascript:ContentClick('label425', 'label424');" onmouseover="ContentPreview('label425');" onmouseout="ContentUnpreview('label425');" title="click to collapse or expand..."> more... </a>
 <div id="label425" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">internet_service_custom</span> - Custom Internet service name list. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: service:id/internet_service_custom:name</span>
 <a id='label426' href="javascript:ContentClick('label427', 'label426');" onmouseover="ContentPreview('label427');" onmouseout="ContentUnpreview('label427');" title="click to collapse or expand..."> more... </a>
 <div id="label427" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>internet_service_custom</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Custom Internet service name. Source firewall.internet-service-custom.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label428' href="javascript:ContentClick('label429', 'label428');" onmouseover="ContentPreview('label429');" onmouseout="ContentUnpreview('label429');" title="click to collapse or expand..."> more... </a>
 <div id="label429" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">internet_service_custom_group</span> - Custom Internet Service group list. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: service:id/internet_service_custom_group:name</span>
 <a id='label430' href="javascript:ContentClick('label431', 'label430');" onmouseover="ContentPreview('label431');" onmouseout="ContentUnpreview('label431');" title="click to collapse or expand..."> more... </a>
 <div id="label431" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>internet_service_custom_group</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Custom Internet Service group name. Source firewall.internet-service-custom-group.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label432' href="javascript:ContentClick('label433', 'label432');" onmouseover="ContentPreview('label433');" onmouseout="ContentUnpreview('label433');" title="click to collapse or expand..."> more... </a>
 <div id="label433" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">internet_service_group</span> - Internet Service group list. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: service:id/internet_service_group:name</span>
 <a id='label434' href="javascript:ContentClick('label435', 'label434');" onmouseover="ContentPreview('label435');" onmouseout="ContentUnpreview('label435');" title="click to collapse or expand..."> more... </a>
 <div id="label435" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>internet_service_group</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Internet Service group name. Source firewall.internet-service-group.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label436' href="javascript:ContentClick('label437', 'label436');" onmouseover="ContentPreview('label437');" onmouseout="ContentUnpreview('label437');" title="click to collapse or expand..."> more... </a>
 <div id="label437" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">internet_service_name</span> - Internet service name list. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: service:id/internet_service_name:name</span>
 <a id='label438' href="javascript:ContentClick('label439', 'label438');" onmouseover="ContentPreview('label439');" onmouseout="ContentUnpreview('label439');" title="click to collapse or expand..."> more... </a>
 <div id="label439" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>internet_service_name</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Internet service name. Source firewall.internet-service-name.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label440' href="javascript:ContentClick('label441', 'label440');" onmouseover="ContentPreview('label441');" onmouseout="ContentUnpreview('label441');" title="click to collapse or expand..."> more... </a>
 <div id="label441" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">jitter_weight</span> - Coefficient of jitter in the formula of custom-profile-1. <span class="li-normal">type: int</span>
 <a id='label442' href="javascript:ContentClick('label443', 'label442');" onmouseover="ContentPreview('label443');" onmouseout="ContentUnpreview('label443');" title="click to collapse or expand..."> more... </a>
 <div id="label443" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>jitter_weight</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">latency_weight</span> - Coefficient of latency in the formula of custom-profile-1. <span class="li-normal">type: int</span>
 <a id='label444' href="javascript:ContentClick('label445', 'label444');" onmouseover="ContentPreview('label445');" onmouseout="ContentUnpreview('label445');" title="click to collapse or expand..."> more... </a>
 <div id="label445" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>latency_weight</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">link_cost_factor</span> - Link cost factor. <span class="li-normal">type: str</span> <span class="li-normal">choices: latency, jitter, packet-loss, inbandwidth, outbandwidth, bibandwidth, custom-profile-1</span>
 <a id='label446' href="javascript:ContentClick('label447', 'label446');" onmouseover="ContentPreview('label447');" onmouseout="ContentUnpreview('label447');" title="click to collapse or expand..."> more... </a>
 <div id="label447" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>link_cost_factor</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[latency]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[jitter]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[packet-loss]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[inbandwidth]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[outbandwidth]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[bibandwidth]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[custom-profile-1]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">link_cost_threshold</span> - Percentage threshold change of link cost values that will result in policy route regeneration (0 - 10000000). <span class="li-normal">type: int</span>
 <a id='label448' href="javascript:ContentClick('label449', 'label448');" onmouseover="ContentPreview('label449');" onmouseout="ContentUnpreview('label449');" title="click to collapse or expand..."> more... </a>
 <div id="label449" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>link_cost_threshold</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">load_balance</span> - Enable/disable load-balance. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label450' href="javascript:ContentClick('label451', 'label450');" onmouseover="ContentPreview('label451');" onmouseout="ContentUnpreview('label451');" title="click to collapse or expand..."> more... </a>
 <div id="label451" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>load_balance</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">minimum_sla_meet_members</span> - Minimum number of members which meet SLA. <span class="li-normal">type: int</span>
 <a id='label452' href="javascript:ContentClick('label453', 'label452');" onmouseover="ContentPreview('label453');" onmouseout="ContentUnpreview('label453');" title="click to collapse or expand..."> more... </a>
 <div id="label453" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>minimum_sla_meet_members</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mode</span> - Control how the SD-WAN rule sets the priority of interfaces in the SD-WAN. <span class="li-normal">type: str</span> <span class="li-normal">choices: auto, manual, priority, sla, load-balance</span>
 <a id='label454' href="javascript:ContentClick('label455', 'label454');" onmouseover="ContentPreview('label455');" onmouseout="ContentUnpreview('label455');" title="click to collapse or expand..."> more... </a>
 <div id="label455" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mode</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[auto]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[manual]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[priority]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[sla]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[load-balance]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v7.4.0</code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">name</span> - SD-WAN rule name. <span class="li-normal">type: str</span>
 <a id='label456' href="javascript:ContentClick('label457', 'label456');" onmouseover="ContentPreview('label457');" onmouseout="ContentUnpreview('label457');" title="click to collapse or expand..."> more... </a>
 <div id="label457" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">packet_loss_weight</span> - Coefficient of packet-loss in the formula of custom-profile-1. <span class="li-normal">type: int</span>
 <a id='label458' href="javascript:ContentClick('label459', 'label458');" onmouseover="ContentPreview('label459');" onmouseout="ContentUnpreview('label459');" title="click to collapse or expand..."> more... </a>
 <div id="label459" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>packet_loss_weight</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">passive_measurement</span> - Enable/disable passive measurement based on the service criteria. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label460' href="javascript:ContentClick('label461', 'label460');" onmouseover="ContentPreview('label461');" onmouseout="ContentUnpreview('label461');" title="click to collapse or expand..."> more... </a>
 <div id="label461" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>passive_measurement</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">priority_members</span> - Member sequence number list. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: service:id/priority_members:seq_num</span>
 <a id='label462' href="javascript:ContentClick('label463', 'label462');" onmouseover="ContentPreview('label463');" onmouseout="ContentUnpreview('label463');" title="click to collapse or expand..."> more... </a>
 <div id="label463" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>priority_members</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">seq_num</span> - Member sequence number. see <a href='#notes'>Notes</a>. Source system.sdwan.members.seq-num. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label464' href="javascript:ContentClick('label465', 'label464');" onmouseover="ContentPreview('label465');" onmouseout="ContentUnpreview('label465');" title="click to collapse or expand..."> more... </a>
 <div id="label465" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>seq_num</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">priority_zone</span> - Priority zone name list. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: service:id/priority_zone:name</span>
 <a id='label466' href="javascript:ContentClick('label467', 'label466');" onmouseover="ContentPreview('label467');" onmouseout="ContentUnpreview('label467');" title="click to collapse or expand..."> more... </a>
 <div id="label467" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>priority_zone</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Priority zone name. Source system.sdwan.zone.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label468' href="javascript:ContentClick('label469', 'label468');" onmouseover="ContentPreview('label469');" onmouseout="ContentUnpreview('label469');" title="click to collapse or expand..."> more... </a>
 <div id="label469" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">protocol</span> - Protocol number. <span class="li-normal">type: int</span>
 <a id='label470' href="javascript:ContentClick('label471', 'label470');" onmouseover="ContentPreview('label471');" onmouseout="ContentUnpreview('label471');" title="click to collapse or expand..."> more... </a>
 <div id="label471" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>protocol</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">quality_link</span> - Quality grade. <span class="li-normal">type: int</span>
 <a id='label472' href="javascript:ContentClick('label473', 'label472');" onmouseover="ContentPreview('label473');" onmouseout="ContentUnpreview('label473');" title="click to collapse or expand..."> more... </a>
 <div id="label473" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>quality_link</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">role</span> - Service role to work with neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: standalone, primary, secondary</span>
 <a id='label474' href="javascript:ContentClick('label475', 'label474');" onmouseover="ContentPreview('label475');" onmouseout="ContentUnpreview('label475');" title="click to collapse or expand..."> more... </a>
 <div id="label475" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>role</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[standalone]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[primary]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[secondary]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">route_tag</span> - IPv4 route map route-tag. <span class="li-normal">type: int</span>
 <a id='label476' href="javascript:ContentClick('label477', 'label476');" onmouseover="ContentPreview('label477');" onmouseout="ContentUnpreview('label477');" title="click to collapse or expand..."> more... </a>
 <div id="label477" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>route_tag</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v7.2.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">shortcut</span> - Enable/disable shortcut for this service. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label478' href="javascript:ContentClick('label479', 'label478');" onmouseover="ContentPreview('label479');" onmouseout="ContentUnpreview('label479');" title="click to collapse or expand..."> more... </a>
 <div id="label479" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>shortcut</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">shortcut_priority</span> - High priority of ADVPN shortcut for this service. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable, auto</span>
 <a id='label480' href="javascript:ContentClick('label481', 'label480');" onmouseover="ContentPreview('label481');" onmouseout="ContentUnpreview('label481');" title="click to collapse or expand..."> more... </a>
 <div id="label481" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>shortcut_priority</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2</code></td>
 <tr>
 <td>[auto]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">shortcut_stickiness</span> - Enable/disable shortcut-stickiness of ADVPN. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label482' href="javascript:ContentClick('label483', 'label482');" onmouseover="ContentPreview('label483');" onmouseout="ContentUnpreview('label483');" title="click to collapse or expand..."> more... </a>
 <div id="label483" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>shortcut_stickiness</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">sla</span> - Service level agreement (SLA). <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: service:id/sla:health_check</span>
 <a id='label484' href="javascript:ContentClick('label485', 'label484');" onmouseover="ContentPreview('label485');" onmouseout="ContentUnpreview('label485');" title="click to collapse or expand..."> more... </a>
 <div id="label485" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sla</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">health_check</span> - SD-WAN health-check. Source system.sdwan.health-check.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label486' href="javascript:ContentClick('label487', 'label486');" onmouseover="ContentPreview('label487');" onmouseout="ContentUnpreview('label487');" title="click to collapse or expand..."> more... </a>
 <div id="label487" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>health_check</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">id</span> - SLA ID. <span class="li-normal">type: int</span>
 <a id='label488' href="javascript:ContentClick('label489', 'label488');" onmouseover="ContentPreview('label489');" onmouseout="ContentUnpreview('label489');" title="click to collapse or expand..."> more... </a>
 <div id="label489" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">sla_compare_method</span> - Method to compare SLA value for SLA mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: order, number</span>
 <a id='label490' href="javascript:ContentClick('label491', 'label490');" onmouseover="ContentPreview('label491');" onmouseout="ContentUnpreview('label491');" title="click to collapse or expand..."> more... </a>
 <div id="label491" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sla_compare_method</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[order]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[number]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">sla_stickiness</span> - Enable/disable SLA stickiness . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label492' href="javascript:ContentClick('label493', 'label492');" onmouseover="ContentPreview('label493');" onmouseout="ContentUnpreview('label493');" title="click to collapse or expand..."> more... </a>
 <div id="label493" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sla_stickiness</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">src</span> - Source address name. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: service:id/src:name</span>
 <a id='label494' href="javascript:ContentClick('label495', 'label494');" onmouseover="ContentPreview('label495');" onmouseout="ContentUnpreview('label495');" title="click to collapse or expand..."> more... </a>
 <div id="label495" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>src</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Address or address group name. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label496' href="javascript:ContentClick('label497', 'label496');" onmouseover="ContentPreview('label497');" onmouseout="ContentUnpreview('label497');" title="click to collapse or expand..."> more... </a>
 <div id="label497" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">src_negate</span> - Enable/disable negation of source address match. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label498' href="javascript:ContentClick('label499', 'label498');" onmouseover="ContentPreview('label499');" onmouseout="ContentUnpreview('label499');" title="click to collapse or expand..."> more... </a>
 <div id="label499" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>src_negate</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">src6</span> - Source address6 name. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: service:id/src6:name</span>
 <a id='label500' href="javascript:ContentClick('label501', 'label500');" onmouseover="ContentPreview('label501');" onmouseout="ContentUnpreview('label501');" title="click to collapse or expand..."> more... </a>
 <div id="label501" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>src6</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Address6 or address6 group name. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label502' href="javascript:ContentClick('label503', 'label502');" onmouseover="ContentPreview('label503');" onmouseout="ContentUnpreview('label503');" title="click to collapse or expand..."> more... </a>
 <div id="label503" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">standalone_action</span> - Enable/disable service when selected neighbor role is standalone while service role is not standalone. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label504' href="javascript:ContentClick('label505', 'label504');" onmouseover="ContentPreview('label505');" onmouseout="ContentUnpreview('label505');" title="click to collapse or expand..."> more... </a>
 <div id="label505" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>standalone_action</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">start_port</span> - Start destination port number. <span class="li-normal">type: int</span>
 <a id='label506' href="javascript:ContentClick('label507', 'label506');" onmouseover="ContentPreview('label507');" onmouseout="ContentUnpreview('label507');" title="click to collapse or expand..."> more... </a>
 <div id="label507" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>start_port</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">start_src_port</span> - Start source port number. <span class="li-normal">type: int</span>
 <a id='label508' href="javascript:ContentClick('label509', 'label508');" onmouseover="ContentPreview('label509');" onmouseout="ContentUnpreview('label509');" title="click to collapse or expand..."> more... </a>
 <div id="label509" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>start_src_port</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">status</span> - Enable/disable SD-WAN service. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label510' href="javascript:ContentClick('label511', 'label510');" onmouseover="ContentPreview('label511');" onmouseout="ContentUnpreview('label511');" title="click to collapse or expand..."> more... </a>
 <div id="label511" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tie_break</span> - Method of selecting member if more than one meets the SLA. <span class="li-normal">type: str</span> <span class="li-normal">choices: zone, cfg-order, fib-best-match, input-device</span>
 <a id='label512' href="javascript:ContentClick('label513', 'label512');" onmouseover="ContentPreview('label513');" onmouseout="ContentUnpreview('label513');" title="click to collapse or expand..."> more... </a>
 <div id="label513" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tie_break</td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[zone]</td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2</code></td>
 <tr>
 <td>[cfg-order]</td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2</code></td>
 <tr>
 <td>[fib-best-match]</td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2</code></td>
 <tr>
 <td>[input-device]</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> 7.6.2</code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tos</span> - Type of service bit pattern. <span class="li-normal">type: str</span>
 <a id='label514' href="javascript:ContentClick('label515', 'label514');" onmouseover="ContentPreview('label515');" onmouseout="ContentUnpreview('label515');" title="click to collapse or expand..."> more... </a>
 <div id="label515" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tos</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tos_mask</span> - Type of service evaluated bits. <span class="li-normal">type: str</span>
 <a id='label516' href="javascript:ContentClick('label517', 'label516');" onmouseover="ContentPreview('label517');" onmouseout="ContentUnpreview('label517');" title="click to collapse or expand..."> more... </a>
 <div id="label517" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tos_mask</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">use_shortcut_sla</span> - Enable/disable use of ADVPN shortcut for quality comparison. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label518' href="javascript:ContentClick('label519', 'label518');" onmouseover="ContentPreview('label519');" onmouseout="ContentUnpreview('label519');" title="click to collapse or expand..."> more... </a>
 <div id="label519" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>use_shortcut_sla</td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">users</span> - User name. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: service:id/users:name</span>
 <a id='label520' href="javascript:ContentClick('label521', 'label520');" onmouseover="ContentPreview('label521');" onmouseout="ContentUnpreview('label521');" title="click to collapse or expand..."> more... </a>
 <div id="label521" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>users</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - User name. Source user.local.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label522' href="javascript:ContentClick('label523', 'label522');" onmouseover="ContentPreview('label523');" onmouseout="ContentUnpreview('label523');" title="click to collapse or expand..."> more... </a>
 <div id="label523" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">zone_mode</span> - Enable/disable zone mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label524' href="javascript:ContentClick('label525', 'label524');" onmouseover="ContentPreview('label525');" onmouseout="ContentUnpreview('label525');" title="click to collapse or expand..."> more... </a>
 <div id="label525" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>zone_mode</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">speedtest_bypass_routing</span> - Enable/disable bypass routing when speedtest on a SD-WAN member. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label526' href="javascript:ContentClick('label527', 'label526');" onmouseover="ContentPreview('label527');" onmouseout="ContentUnpreview('label527');" title="click to collapse or expand..."> more... </a>
 <div id="label527" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>speedtest_bypass_routing</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">status</span> - Enable/disable SD-WAN. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label528' href="javascript:ContentClick('label529', 'label528');" onmouseover="ContentPreview('label529');" onmouseout="ContentUnpreview('label529');" title="click to collapse or expand..."> more... </a>
 <div id="label529" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">zone</span> - Configure SD-WAN zones. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: zone:name</span>
 <a id='label530' href="javascript:ContentClick('label531', 'label530');" onmouseover="ContentPreview('label531');" onmouseout="ContentUnpreview('label531');" title="click to collapse or expand..."> more... </a>
 <div id="label531" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>zone</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">advpn_health_check</span> - Health check for ADVPN local overlay link quality. Source system.sdwan.health-check.name. <span class="li-normal">type: str</span>
 <a id='label532' href="javascript:ContentClick('label533', 'label532');" onmouseover="ContentPreview('label533');" onmouseout="ContentUnpreview('label533');" title="click to collapse or expand..."> more... </a>
 <div id="label533" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>advpn_health_check</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">advpn_select</span> - Enable/disable selection of ADVPN based on SDWAN information. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label534' href="javascript:ContentClick('label535', 'label534');" onmouseover="ContentPreview('label535');" onmouseout="ContentUnpreview('label535');" title="click to collapse or expand..."> more... </a>
 <div id="label535" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>advpn_select</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">minimum_sla_meet_members</span> - Minimum number of members which meet SLA when the neighbor is preferred. <span class="li-normal">type: int</span>
 <a id='label536' href="javascript:ContentClick('label537', 'label536');" onmouseover="ContentPreview('label537');" onmouseout="ContentUnpreview('label537');" title="click to collapse or expand..."> more... </a>
 <div id="label537" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>minimum_sla_meet_members</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">name</span> - Zone name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label538' href="javascript:ContentClick('label539', 'label538');" onmouseover="ContentPreview('label539');" onmouseout="ContentUnpreview('label539');" title="click to collapse or expand..."> more... </a>
 <div id="label539" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">service_sla_tie_break</span> - Method of selecting member if more than one meets the SLA. <span class="li-normal">type: str</span> <span class="li-normal">choices: cfg-order, fib-best-match, input-device</span>
 <a id='label540' href="javascript:ContentClick('label541', 'label540');" onmouseover="ContentPreview('label541');" onmouseout="ContentUnpreview('label541');" title="click to collapse or expand..."> more... </a>
 <div id="label541" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>service_sla_tie_break</td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[cfg-order]</td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2</code></td>
 <tr>
 <td>[fib-best-match]</td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2</code></td>
 <tr>
 <td>[input-device]</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> 7.6.2</code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
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
    
    - name: Configure redundant Internet connections with multiple outbound links and health-check profiles.
      fortinet.fortios.fortios_system_sdwan:
          vdom: "{{ vdom }}"
          system_sdwan:
              app_perf_log_period: "0"
              duplication:
                  -
                      dstaddr:
                          -
                              name: "default_name_6 (source firewall.address.name firewall.addrgrp.name)"
                      dstaddr6:
                          -
                              name: "default_name_8 (source firewall.address6.name firewall.addrgrp6.name)"
                      dstintf:
                          -
                              name: "default_name_10 (source system.interface.name system.zone.name system.sdwan.zone.name)"
                      id: "11"
                      packet_de_duplication: "enable"
                      packet_duplication: "disable"
                      service:
                          -
                              name: "default_name_15 (source firewall.service.custom.name firewall.service.group.name)"
                      service_id:
                          -
                              id: "17 (source system.sdwan.service.id)"
                      sla_match_service: "enable"
                      srcaddr:
                          -
                              name: "default_name_20 (source firewall.address.name firewall.addrgrp.name)"
                      srcaddr6:
                          -
                              name: "default_name_22 (source firewall.address6.name firewall.addrgrp6.name)"
                      srcintf:
                          -
                              name: "default_name_24 (source system.interface.name system.zone.name system.sdwan.zone.name)"
              duplication_max_discrepancy: "250"
              duplication_max_num: "2"
              fail_alert_interfaces:
                  -
                      name: "default_name_28 (source system.interface.name)"
              fail_detect: "enable"
              health_check:
                  -
                      addr_mode: "ipv4"
                      class_id: "0"
                      detect_mode: "active"
                      diffservcode: "<your_own_value>"
                      dns_match_ip: "<your_own_value>"
                      dns_request_domain: "<your_own_value>"
                      embed_measured_health: "enable"
                      failtime: "5"
                      fortiguard: "disable"
                      fortiguard_name: "<your_own_value> (source system.health-check-fortiguard.name)"
                      ftp_file: "<your_own_value>"
                      ftp_mode: "passive"
                      ha_priority: "1"
                      http_agent: "<your_own_value>"
                      http_get: "<your_own_value>"
                      http_match: "<your_own_value>"
                      interval: "500"
                      members:
                          -
                              seq_num: "<you_own_value>"
                      mos_codec: "g711"
                      name: "default_name_51"
                      packet_size: "124"
                      password: "<your_own_value>"
                      port: "0"
                      probe_count: "30"
                      probe_packets: "disable"
                      probe_timeout: "500"
                      protocol: "ping"
                      quality_measured_method: "half-open"
                      recoverytime: "5"
                      security_mode: "none"
                      server: "192.168.100.40"
                      sla:
                          -
                              id: "64"
                              jitter_threshold: "5"
                              latency_threshold: "5"
                              link_cost_factor: "latency"
                              mos_threshold: "<your_own_value>"
                              packetloss_threshold: "0"
                              priority_in_sla: "0"
                              priority_out_sla: "0"
                      sla_fail_log_period: "0"
                      sla_id_redistribute: "0"
                      sla_pass_log_period: "0"
                      source: "<your_own_value>"
                      source6: "<your_own_value>"
                      system_dns: "disable"
                      threshold_alert_jitter: "0"
                      threshold_alert_latency: "0"
                      threshold_alert_packetloss: "0"
                      threshold_warning_jitter: "0"
                      threshold_warning_latency: "0"
                      threshold_warning_packetloss: "0"
                      update_cascade_interface: "enable"
                      update_static_route: "enable"
                      user: "<your_own_value>"
                      vrf: "0"
              health_check_fortiguard:
                  -
                      addr_mode: "ipv4"
                      class_id: "0"
                      detect_mode: "active"
                      diffservcode: "<your_own_value>"
                      dns_match_ip: "<your_own_value>"
                      dns_request_domain: "<your_own_value>"
                      embed_measured_health: "enable"
                      failtime: "5"
                      ftp_file: "<your_own_value>"
                      ftp_mode: "passive"
                      ha_priority: "1"
                      http_agent: "<your_own_value>"
                      http_get: "<your_own_value>"
                      http_match: "<your_own_value>"
                      interval: "500"
                      members:
                          -
                              seq_num: "<you_own_value>"
                      mos_codec: "g711"
                      packet_size: "124"
                      password: "<your_own_value>"
                      port: "0"
                      probe_count: "30"
                      probe_packets: "disable"
                      probe_timeout: "500"
                      protocol: "ping"
                      quality_measured_method: "half-open"
                      recoverytime: "5"
                      security_mode: "none"
                      server: "192.168.100.40"
                      sla:
                          -
                              id: "119"
                              jitter_threshold: "5"
                              latency_threshold: "5"
                              link_cost_factor: "latency"
                              mos_threshold: "<your_own_value>"
                              packetloss_threshold: "0"
                              priority_in_sla: "0"
                              priority_out_sla: "0"
                      sla_fail_log_period: "0"
                      sla_id_redistribute: "0"
                      sla_pass_log_period: "0"
                      source: "<your_own_value>"
                      source6: "<your_own_value>"
                      system_dns: "disable"
                      target_name: "<your_own_value>"
                      threshold_alert_jitter: "0"
                      threshold_alert_latency: "0"
                      threshold_alert_packetloss: "0"
                      threshold_warning_jitter: "0"
                      threshold_warning_latency: "0"
                      threshold_warning_packetloss: "0"
                      update_cascade_interface: "enable"
                      update_static_route: "enable"
                      user: "<your_own_value>"
                      vrf: "0"
              load_balance_mode: "source-ip-based"
              members:
                  -
                      comment: "Comments."
                      cost: "0"
                      gateway: "<your_own_value>"
                      gateway6: "<your_own_value>"
                      ingress_spillover_threshold: "0"
                      interface: "<your_own_value> (source system.interface.name)"
                      preferred_source: "<your_own_value>"
                      priority: "1"
                      priority_in_sla: "0"
                      priority_out_sla: "0"
                      priority6: "1024"
                      seq_num: "<you_own_value>"
                      source: "<your_own_value>"
                      source6: "<your_own_value>"
                      spillover_threshold: "0"
                      status: "disable"
                      transport_group: "0"
                      volume_ratio: "1"
                      weight: "1"
                      zone: "<your_own_value> (source system.sdwan.zone.name)"
              neighbor:
                  -
                      health_check: "<your_own_value> (source system.sdwan.health-check.name)"
                      ip: "<your_own_value> (source router.bgp.neighbor-group.name router.bgp.neighbor.ip)"
                      member:
                          -
                              seq_num: "<you_own_value>"
                      minimum_sla_meet_members: "1"
                      mode: "sla"
                      role: "standalone"
                      route_metric: "preferable"
                      service_id: "0"
                      sla_id: "0"
              neighbor_hold_boot_time: "0"
              neighbor_hold_down: "enable"
              neighbor_hold_down_time: "0"
              service:
                  -
                      addr_mode: "ipv4"
                      agent_exclusive: "enable"
                      bandwidth_weight: "0"
                      comment: "Comments."
                      default: "enable"
                      dscp_forward: "enable"
                      dscp_forward_tag: "<your_own_value>"
                      dscp_reverse: "enable"
                      dscp_reverse_tag: "<your_own_value>"
                      dst:
                          -
                              name: "default_name_191 (source firewall.address.name firewall.addrgrp.name)"
                      dst_negate: "enable"
                      dst6:
                          -
                              name: "default_name_194 (source firewall.address6.name firewall.addrgrp6.name)"
                      end_port: "65535"
                      end_src_port: "65535"
                      gateway: "enable"
                      groups:
                          -
                              name: "default_name_199 (source user.group.name)"
                      hash_mode: "round-robin"
                      health_check:
                          -
                              name: "default_name_202 (source system.sdwan.health-check.name)"
                      hold_down_time: "0"
                      id: "204"
                      input_device:
                          -
                              name: "default_name_206 (source system.interface.name)"
                      input_device_negate: "enable"
                      input_zone:
                          -
                              name: "default_name_209 (source system.sdwan.zone.name)"
                      internet_service: "enable"
                      internet_service_app_ctrl:
                          -
                              id: "212"
                      internet_service_app_ctrl_category:
                          -
                              id: "214"
                      internet_service_app_ctrl_group:
                          -
                              name: "default_name_216 (source application.group.name)"
                      internet_service_custom:
                          -
                              name: "default_name_218 (source firewall.internet-service-custom.name)"
                      internet_service_custom_group:
                          -
                              name: "default_name_220 (source firewall.internet-service-custom-group.name)"
                      internet_service_group:
                          -
                              name: "default_name_222 (source firewall.internet-service-group.name)"
                      internet_service_name:
                          -
                              name: "default_name_224 (source firewall.internet-service-name.name)"
                      jitter_weight: "0"
                      latency_weight: "0"
                      link_cost_factor: "latency"
                      link_cost_threshold: "10"
                      load_balance: "enable"
                      minimum_sla_meet_members: "0"
                      mode: "auto"
                      name: "default_name_232"
                      packet_loss_weight: "0"
                      passive_measurement: "enable"
                      priority_members:
                          -
                              seq_num: "<you_own_value>"
                      priority_zone:
                          -
                              name: "default_name_238 (source system.sdwan.zone.name)"
                      protocol: "0"
                      quality_link: "0"
                      role: "standalone"
                      route_tag: "0"
                      shortcut: "enable"
                      shortcut_priority: "enable"
                      shortcut_stickiness: "enable"
                      sla:
                          -
                              health_check: "<your_own_value> (source system.sdwan.health-check.name)"
                              id: "248"
                      sla_compare_method: "order"
                      sla_stickiness: "enable"
                      src:
                          -
                              name: "default_name_252 (source firewall.address.name firewall.addrgrp.name)"
                      src_negate: "enable"
                      src6:
                          -
                              name: "default_name_255 (source firewall.address6.name firewall.addrgrp6.name)"
                      standalone_action: "enable"
                      start_port: "1"
                      start_src_port: "1"
                      status: "enable"
                      tie_break: "zone"
                      tos: "<your_own_value>"
                      tos_mask: "<your_own_value>"
                      use_shortcut_sla: "enable"
                      users:
                          -
                              name: "default_name_265 (source user.local.name)"
                      zone_mode: "enable"
              speedtest_bypass_routing: "disable"
              status: "disable"
              zone:
                  -
                      advpn_health_check: "<your_own_value> (source system.sdwan.health-check.name)"
                      advpn_select: "enable"
                      minimum_sla_meet_members: "1"
                      name: "default_name_273"
                      service_sla_tie_break: "cfg-order"


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
