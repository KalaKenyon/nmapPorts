# Custom Nmap Scan Script

<p>Custom Nmap Scan Script is a Bash script designed for performing targeted Nmap scans on specific ports of your choosing, of a specified IP address.</p>

<p><strong>NOTE:</strong> This script was created to suplement my personal learning for the PNPT exam.</p>

<h2>How it Works</h2>

<ol>
  <li><strong>User Interaction:</strong> Run the script and input your target IP address.</li>
  <li><strong>Scan Execution:</strong> The script performs an Nmap scan on the specified ports.</li>
  <li><strong>Result Display:</strong> View the scan results to identify open ports and services.</li>
</ol>

<h2>Usage</h2>

<ol>
  <li>Clone the repository or download the <code>custom_nmap_scan.sh</code> file.</li>
  <li>Open a terminal window and navigate to the directory containing <code>custom_nmap_scan.sh</code>.</li>
  <li>Make the script executable by running the following command:</li>
</ol>

<pre><code>chmod +x custom_nmap_scan.sh</code></pre>

<ol start="4">
  <li>Run the script with the following command:</li>
</ol>

<pre><code>./custom_nmap_scan.sh</code></pre>

<h2>Parameters</h2>

<ul>
  <li><strong><code>target_ip:</code></strong> Set the target IP address you want to scan in the <code>custom_nmap_scan.sh</code> script.</li>
  <li><strong><code>ports:</code></strong> Specify the ports you want to scan in the <code>custom_nmap_scan.sh</code> script. By default, it scans ports 22, 80, 139, and 443.</li>
</ul>

<h2>Example</h2>

<pre><code>#!/bin/bash

# Define the target IP address
target_ip="xxx.xxx.xxx.xxx"

# Define the ports to scan
ports="22,80,139,443"

# Run Nmap scan with specified options
nmap -T4 -p$ports -A $target_ip

# End of script
</code></pre>

<h2>License</h2>

<p>None</p>

<h2>Contributing</h2>

<p>Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.</p>

<h2>Acknowledgements</h2>

<p>The Custom Nmap Scan Script simplifies the process of conducting targeted Nmap scans for cybersecurity purposes.</p>

<h2>Disclaimer</h2>

<p>This tool should be used responsibly and for educational purposes only. The author is not responsible for any misuse or damage caused by this software.</p>

<h2>Contact</h2>

<p>For any inquiries, please contact <a href="https://github.com/KalaKenyon">Kala Kenyon</a>.</p>
