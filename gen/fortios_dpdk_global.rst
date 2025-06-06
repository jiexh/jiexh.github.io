:source: fortios_dpdk_global.py

:orphan:

.. fortios_dpdk_global:

fortios_dpdk_global -- Configure global DPDK options in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify dpdk feature and global category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.15


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------
Supported Version Ranges: v7.0.0 -> v7.0.12, v7.2.1 -> v7.2.2, v7.4.0 -> v7.6.1


Parameters
----------


.. raw:: html

    <ul>
    <li> <span class="li-head">access_token</span> - Token-based authentication. Generated from GUI of Fortigate. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> </li>
    <li> <span class="li-head">enable_log</span> - Enable/Disable logging for task. <span class="li-normal">type: bool</span> <span class="li-required">required: false</span> <span class="li-normal">default: False</span> </li>
    <li> <span class="li-head">vdom</span> - Virtual domain, among those defined previously. A vdom is a virtual instance of the FortiGate that can be configured and used as a different unit. <span class="li-normal">type: str</span> <span class="li-normal">default: root</span> </li>
    <li> <span class="li-head">member_path</span> - Member attribute path to operate on. <span class="li-normal">type: str</span> </li>
    <li> <span class="li-head">member_state</span> - Add or delete a member under specified attribute path. <span class="li-normal">type: str</span> <span class="li-normal">choices: present, absent</span> </li>
    <li> <span class="li-head">dpdk_global</span> - Configure global DPDK options. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dpdk_global</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.6.1 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">elasticbuffer</span> - Enable/disable elasticbuffer support for all DPDK ports. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>elasticbuffer</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.6.1 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.0.12</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.0.12</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">hugepage_percentage</span> - Percentage of main memory allocated to hugepages, which are available for DPDK operation. <span class="li-normal">type: int</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>hugepage_percentage</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.6.1 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">interface</span> - Physical interfaces that enable DPDK. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: interface:interface_name</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>interface</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.6.1 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">interface_name</span> - Physical interface name. Source system.interface.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>interface_name</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.6.1 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">ipsec_offload</span> - Enable/disable DPDK IPsec phase 2 offloading. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipsec_offload</td>
 <td><code class="docutils literal notranslate">v7.0.6 -> v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.6.1 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.0.6 -> v7.0.12</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.0.6 -> v7.0.12</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">mbufpool_percentage</span> - Percentage of main memory allocated to DPDK packet buffer. <span class="li-normal">type: int</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mbufpool_percentage</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.6.1 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">multiqueue</span> - Enable/disable multi-queue RX/TX support for all DPDK ports. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>multiqueue</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.6.1 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.0.12</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.0.12</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">per_session_accounting</span> - Enable/disable per-session accounting. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, traffic-log-only, enable</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>per_session_accounting</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.6.1 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.0.12</code></td>
 <tr>
 <td>[traffic-log-only]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.0.12</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.0.12</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">protects</span> - Special arguments for device <span class="li-normal">type: str</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>protects</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.6.1 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">session_table_percentage</span> - Percentage of main memory allocated to DPDK session table. <span class="li-normal">type: int</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>session_table_percentage</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> v7.6.1 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">sleep_on_idle</span> - Enable/disable sleep-on-idle support for all FDH engines. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sleep_on_idle</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.6.1 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.0.12</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.0.12</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">status</span> - Enable/disable DPDK operation for the entire system. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.6.1 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.0.12</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.0.12</code></td>
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
    
    - name: Configure global DPDK options.
      fortinet.fortios.fortios_dpdk_global:
          vdom: "{{ vdom }}"
          dpdk_global:
              elasticbuffer: "disable"
              hugepage_percentage: "30"
              interface:
                  -
                      interface_name: "<your_own_value> (source system.interface.name)"
              ipsec_offload: "disable"
              mbufpool_percentage: "25"
              multiqueue: "disable"
              per_session_accounting: "disable"
              protects: "<your_own_value>"
              session_table_percentage: "5"
              sleep_on_idle: "disable"
              status: "disable"


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
