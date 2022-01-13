## **seb-patch**: Use **SEB** in any VM (**VirtualBox**, **VMWare**, ...)

### _That's it-_

#

<details>
  <summary><b>How does this work?</b> (Click to expand/collapse)</summary>
    <b><i>Coming Soon!</i></b>
</details>

<br />

<details>
  <summary><b>FAQ</b> (Click to expand/collapse)</summary>
  <b>Q1: Does my exam organizer/teacher get notified if I'm using a Virtual Machine?</b><br>
  <b>A: Short answer is no</b>. <i>Although, in theory, those that are more <b>tech-savvy</b>, could ask for your SEB logs</i>.
  <br />
  <br />
  
  From <a href="https://safeexambrowser.org/about_overview_en.html#privacy-statement">SEB Official Website</a>:
  <blockquote>
    <i>[...]</i> Some data which can be considered to be personal (<b>computer host name</b>, <b>computer account user name</b>, some URLs of opened web pages etc.) can be <b>contained in the log files SEB saves on the system it is running on</b> (when used with default settings). <b>Log files are not transmitted to any server</b> by SEB, <b>you can manually collect those log files for debugging purposes.</b>
  </blockquote>
  
  <b>Q2: What can my exam organizer/teacher do with my SEB logs anyways?</b><br />
  <b>A:</b> Welp, surprisingly... Not much from what we analyzed. Although they can always obtain <i>as referred on the quote before</i> your <b>computer hostname</b> and <b>account user name</b>. If you're running SEB on a virtual machine, obviously, that it's not going to match your original laptop's model or <i>even a valid computer model in that matter</i>. Example below.

<i>(<code>YYYY-MM-DD</code>\_<code>hh:mm:ss</code>\_Runtime.log @ Line 7):</i>
<br />

  <table>
    <tr>
      <th>Running SEB on a</th>
      <th>Output</th>
      <th>Expected Output</th>
    </tr>
    <tr>
      <td>Laptop</td>
      <td>Computer 'DESKTOP-1B2D3F4' is a <b>Zenbook Pro 15 UX550</b> manufactured by <b>Asus</b></td>
      <td align="center">✅</td>
    </tr>
    <tr>
      <td>Virtual Machine (<b>VirtualBox</b>)</td>
      <td>Computer 'DESKTOP-1A2C3E4' is a <b>Virtual Machine VirtualBox</b> manufactured by <b>innotek GmbH</b></td>
      <td align="center">❌</td></center>
    </tr>
  </table>
    
  <b><i>Coming Soon!</i></b><br />
  <b>Q̶3̶:̶ ̶W̶h̶a̶t̶ ̶i̶f̶ ̶m̶y̶ ̶e̶x̶a̶m̶ ̶o̶r̶g̶a̶n̶i̶z̶e̶r̶/̶t̶e̶a̶c̶h̶e̶r̶ ̶d̶o̶e̶s̶ ̶a̶s̶k̶ ̶f̶o̶r̶ ̶m̶y̶ ̶S̶E̶B̶ ̶l̶o̶g̶s̶ ̶a̶f̶t̶e̶r̶ ̶m̶y̶ ̶e̶x̶a̶m̶/̶t̶e̶s̶t̶?̶ ̶A̶m̶ ̶I̶ ̶d̶o̶o̶m̶e̶d̶?̶</b>
  <br />
  <b>A:</b> No, don't panic. In this repository @ the folder <code>\logs</code> we provide a solution to this problem.
 </details>
