<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com/watch?v=WRr7XhbUlJg)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

<div class="markdown prose w-full break-words dark:prose-invert light"></p><ol><li><p><strong>Server Requirements</strong>:</p><ul><li>Linux, Windows, or macOS (Linux preferred for production).</li><li>Web Server: Apache 2.4+ or Nginx.</li></ul></li><li><p><strong>PHP Requirements</strong>:</p><ul><li>PHP 7.4 to 8.0 (not compatible with PHP 8.1 or later).</li><li>Required extensions:<ul><li><code>mysqli</code></li><li><code>gd</code></li><li><code>gettext</code></li><li><code>imap</code></li><li><code>mbstring</code></li><li><code>xml</code></li><li><code>json</code></li><li><code>intl</code></li><li><code>phar</code></li><li><code>fileinfo</code></li></ul></li></ul></li><li><p><strong>Database</strong>:</p><ul><li>MySQL 5.5+ or MariaDB 10.0+.</li><li>Ability to create and manage a database.</li></ul></li><li><p><strong>Optional (but recommended)</strong>:</p><ul><li>SMTP server for email notifications.</li></ul></li><li><p><strong>Download osTicket</strong>:</p><ul><li>Get the latest osTicket version from <a rel="noopener" target="_new" style="--streaming-animation-state: var(--batch-play-state-1); --animation-rate: var(--batch-play-rate-1);"><span style="--animation-count: 3; --streaming-animation-state: var(--batch-play-state-2);">osTicket's</span><span style="--animation-count: 4; --streaming-animation-state: var(--batch-play-state-2);"> website</span></a>.</li></ul></li><li><p><strong>Recommended Hardware</strong>:</p><ul><li>CPU: 1 GHz+</li><li>RAM: 2 GB minimum</li><li>Storage: 5 GB minimum</li></ul></li><li><p><strong>Installation Steps</strong>:</p><ul><li>Upload osTicket files to your server.</li><li>Create a MySQL or MariaDB database and user.</li><li>Complete web-based setup via your server’s URL.</li><li>Configure email, ticket settings, and user permissions in the admin panel.</li></ul></li></ol><p>






<h2>Installation Steps</h2>

<p>
  
![Screenshot (7)](https://github.com/user-attachments/assets/c0a05d6c-4cac-4021-91eb-e0db2534c335)


  
</p>
<p>
Step #1: Upload osTicket files to your server. If you're using a tool like <strong>FileZilla</strong> or another FTP client, you should see the files from the osTicket download (folders like <code>include</code>, <code>setup</code>, etc.) being uploaded to your server’s root directory, typically <code>/var/www/html</code> or another web-accessible directory.
</p>
<br />

<p>
  
![Screenshot (9)](https://github.com/user-attachments/assets/581d3cbf-b6d7-49c1-b218-826a7bbd7065)


</p>
<p>
Step #2: Create a MySQL or MariaDB Database and User. In phpMyAdmin, after logging in, select "Databases" &gt; "Create Database," where you’ll enter the database name for osTicket. You should then see an interface for creating a user with specific permissions for the new database.
</p>
<br />

<p>
  
![Screenshot (8)](https://github.com/user-attachments/assets/ad9cd176-d92d-4675-9f09-2a0e38eb5443)


</p>
<p>
Step #3: Start osTicket web-based setup. Navigate to your server’s URL (e.g., <code>http://yourdomain.com/upload/</code>). You’ll see the <strong>osTicket Installer</strong> page with a welcome message, listing system requirements and an option to continue with the installation if all prerequisites are met. If any requirements are missing (e.g., PHP extensions), they will appear in red with instructions on fixing them.
</p>
<br />

<p>
  
![Screenshot (10)](https://github.com/user-attachments/assets/b21d3b1e-e5a7-4607-a243-94006f6a16c2)


</p>
<p>
Step #4: Configuration in the osTicket Admin Panel. After logging into the admin panel, you’ll see a dashboard with options for configuring <strong>Email Settings</strong>, <strong>Ticket Settings</strong>, <strong>Departments</strong>, <strong>Teams</strong>, and more. You can click on each option to configure details like email piping for ticket replies, SLA policies, and user permissions.
</p>
<br />

