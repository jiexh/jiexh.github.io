:source: fortios_firewall_local_in_policy.py

:orphan:

.. fortios_firewall_local_in_policy:

fortios_firewall_local_in_policy -- Configure user defined IPv4 local-in policies in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify firewall feature and local_in_policy category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">state</span> - Indicates whether to create or remove the object. <span class="li-normal">type: str</span> <span class="li-required">required: true</span> <span class="li-normal">choices: present, absent</span> </li>
    <li> <span class="li-head">firewall_local_in_policy</span> - Configure user defined IPv4 local-in policies. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>firewall_local_in_policy</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">action</span> - Action performed on traffic matching the policy . <span class="li-normal">type: str</span> <span class="li-normal">choices: accept, deny</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>action</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[accept]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">comments</span> - Comment. <span class="li-normal">type: str</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>comments</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dstaddr</span> - Destination address object from available options. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: dstaddr:name</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dstaddr</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address.name firewall.addrgrp.name system.external-resource.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">dstaddr_negate</span> - When enabled dstaddr specifies what the destination address must NOT be. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dstaddr_negate</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ha_mgmt_intf_only</span> - Enable/disable dedicating the HA management interface only for local-in policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ha_mgmt_intf_only</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">internet_service_src</span> - Enable/disable use of Internet Services in source for this local-in policy. If enabled, source address is not used. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>internet_service_src</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">internet_service_src_custom</span> - Custom Internet Service source name. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: internet_service_src_custom:name</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>internet_service_src_custom</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Custom Internet Service name. Source firewall.internet-service-custom.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">internet_service_src_custom_group</span> - Custom Internet Service source group name. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: internet_service_src_custom_group:name</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>internet_service_src_custom_group</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Custom Internet Service group name. Source firewall.internet-service-custom-group.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">internet_service_src_group</span> - Internet Service source group name. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: internet_service_src_group:name</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>internet_service_src_group</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Internet Service group name. Source firewall.internet-service-group.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">internet_service_src_name</span> - Internet Service source name. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: internet_service_src_name:name</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>internet_service_src_name</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Internet Service name. Source firewall.internet-service-name.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">internet_service_src_negate</span> - When enabled internet-service-src specifies what the service must NOT be. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>internet_service_src_negate</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">intf</span> - Incoming interface name from available options. Source system.zone.name system.interface.name. <span class="li-normal">type: str</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>intf</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.1 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">intf_dict</span> - Incoming interface name from available options. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: intf_dict:name</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>intf_dict</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source system.zone.name system.sdwan.zone.name system.interface.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">logtraffic</span> - Enable/disable local-in traffic logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>logtraffic</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">policyid</span> - User defined local in policy ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>policyid</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">schedule</span> - Schedule object from available options. Source firewall.schedule.onetime.name firewall.schedule.recurring.name firewall.schedule.group .name. <span class="li-normal">type: str</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>schedule</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">service</span> - Service object from available options. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: service:name</span>
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>service</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Service name. Source firewall.service.custom.name firewall.service.group.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">service_negate</span> - When enabled service specifies what the service must NOT be. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>service_negate</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">srcaddr</span> - Source address object from available options. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: srcaddr:name</span>
 <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>srcaddr</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address.name firewall.addrgrp.name system.external-resource.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label54' href="javascript:ContentClick('label55', 'label54');" onmouseover="ContentPreview('label55');" onmouseout="ContentUnpreview('label55');" title="click to collapse or expand..."> more... </a>
 <div id="label55" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">srcaddr_negate</span> - When enabled srcaddr specifies what the source address must NOT be. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label56' href="javascript:ContentClick('label57', 'label56');" onmouseover="ContentPreview('label57');" onmouseout="ContentUnpreview('label57');" title="click to collapse or expand..."> more... </a>
 <div id="label57" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>srcaddr_negate</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">status</span> - Enable/disable this local-in policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label58' href="javascript:ContentClick('label59', 'label58');" onmouseover="ContentPreview('label59');" onmouseout="ContentUnpreview('label59');" title="click to collapse or expand..."> more... </a>
 <div id="label59" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">uuid</span> - Universally Unique Identifier (UUID; automatically assigned but can be manually reset). <span class="li-normal">type: str</span>
 <a id='label60' href="javascript:ContentClick('label61', 'label60');" onmouseover="ContentPreview('label61');" onmouseout="ContentUnpreview('label61');" title="click to collapse or expand..."> more... </a>
 <div id="label61" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>uuid</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">virtual_patch</span> - Enable/disable virtual patching. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label62' href="javascript:ContentClick('label63', 'label62');" onmouseover="ContentPreview('label63');" onmouseout="ContentUnpreview('label63');" title="click to collapse or expand..."> more... </a>
 <div id="label63" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>virtual_patch</td>
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
        </ul>
    </ul>


Notes
-----

.. note::

   - We highly recommend using your own value as the policyid instead of 0, while '0' is a special placeholder that allows the backend to assign the latest available number for the object, it does have limitations. Please find more details in Q&A.

   - Legacy fortiosapi has been deprecated, httpapi is the preferred way to run playbooks

   - The module supports check_mode.



Examples
--------

.. code-block:: yaml+jinja
    
    - name: Configure user defined IPv4 local-in policies.
      fortinet.fortios.fortios_firewall_local_in_policy:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          firewall_local_in_policy:
              action: "accept"
              comments: "<your_own_value>"
              dstaddr:
                  -
                      name: "default_name_6 (source firewall.address.name firewall.addrgrp.name system.external-resource.name)"
              dstaddr_negate: "enable"
              ha_mgmt_intf_only: "enable"
              internet_service_src: "enable"
              internet_service_src_custom:
                  -
                      name: "default_name_11 (source firewall.internet-service-custom.name)"
              internet_service_src_custom_group:
                  -
                      name: "default_name_13 (source firewall.internet-service-custom-group.name)"
              internet_service_src_group:
                  -
                      name: "default_name_15 (source firewall.internet-service-group.name)"
              internet_service_src_name:
                  -
                      name: "default_name_17 (source firewall.internet-service-name.name)"
              internet_service_src_negate: "enable"
              intf: "<your_own_value> (source system.zone.name system.interface.name)"
              intf_dict:
                  -
                      name: "default_name_21 (source system.zone.name system.sdwan.zone.name system.interface.name)"
              logtraffic: "enable"
              policyid: "<you_own_value>"
              schedule: "<your_own_value> (source firewall.schedule.onetime.name firewall.schedule.recurring.name firewall.schedule.group.name)"
              service:
                  -
                      name: "default_name_26 (source firewall.service.custom.name firewall.service.group.name)"
              service_negate: "enable"
              srcaddr:
                  -
                      name: "default_name_29 (source firewall.address.name firewall.addrgrp.name system.external-resource.name)"
              srcaddr_negate: "enable"
              status: "enable"
              uuid: "<your_own_value>"
              virtual_patch: "enable"


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
