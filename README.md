

# PowerShell in Cybersecurity: Working Smarter Through Automation



## Introduction



Cybersecurity is not just about stopping hackers. It is also about understanding how computer systems work, identifying potential problems, and finding ways to keep those systems secure.



One tool I have been learning to use is **Windows PowerShell**. It allows administrators and cybersecurity professionals to manage systems, investigate issues, and automate tasks.



What interests me most is how a few lines of code can replace tasks that would otherwise take much longer to complete manually.



## Why PowerShell Matters



PowerShell is a *command-line shell and scripting language* developed by Microsoft.



Instead of manually clicking through Windows settings, administrators can use commands to gather information, manage services, and perform repetitive tasks.



### Benefits of PowerShell



- **Automation:** Reduce repetitive manual work.

- **Efficiency:** Complete administrative tasks faster.

- **Consistency:** Perform the same procedure across multiple systems.

- **Security Monitoring:** Examine processes, services, and event logs.

- **Remote Administration:** Manage systems without physically accessing them.



> "Automation is useful, but understanding what a script does is just as important as running it."

>

> This is something I try to remember while learning PowerShell.



## How I Use PowerShell



### 1. Checking Running Processes



The following command displays processes currently running on a Windows computer:



`Get-Process`



This can help identify unfamiliar programs or processes consuming excessive resources.



### 2. Checking Windows Services



To display services on a computer, I can use:



`Get-Service`



I can also filter the results to show only running services.



```powershell

Get-Service | Where-Object Status -eq 'Running'

```



### 3. Reviewing Security Events



PowerShell can also retrieve Windows security events.



```powershell

Get-WinEvent -LogName Security -MaxEvents 5

```



This command requests the five most recent entries from the Security event log. Access may require administrator permissions.



## My Cybersecurity Workflow



When investigating a potential issue, I would follow an organized process:



1. Identify the problem.

2. Gather system information.

     1. Check running processes.

     2. Review Windows services.

     3. Examine relevant event logs.

3. Investigate anything unusual.

4. Document my findings.

5. Recommend appropriate corrective actions.



Following a process helps me avoid jumping to conclusions before collecting evidence.



## PowerShell Commands Reference




| Command | Purpose | Security Application |
|:--------|:-------:|---------------------:|
| `Get-Process` | Lists running processes | Identify suspicious activity |
| `Get-Service` | Displays Windows services | Review active services |
| `Get-WinEvent` | Reads Windows event logs | Investigate security events |
| `Get-NetTCPConnection` | Shows TCP connections | Examine network activity |
| `Get-LocalUser` | Lists local user accounts | Review local identities |




## Good Security Practices



When using PowerShell, I think it is important to follow these guidelines:



- Review scripts before executing them.

- Avoid using administrator privileges unnecessarily.

- Never place passwords directly inside scripts.

- Test unfamiliar scripts in a safe environment.

       - Use a virtual machine when appropriate.

       - Record errors and troubleshooting steps.

- Document changes so they can be reviewed later.



## My Learning Checklist



- [x] Install PowerShell and Git.

- [x] Create a local Git repository.

- [x] Create a README.md file.

- [x ] Commit the Markdown article to Git.

- [x ] Complete the PowerShell ImportExcel lab.

- [x ] Document commands, outputs, and screenshots.

- [ ] Complete the final lab report.



## Helpful Learning Resources



The following resources are useful when learning PowerShell, Git, and Markdown:



- [Microsoft PowerShell Documentation](https://learn.microsoft.com/powershell/)

- [Markdown Basic Syntax Guide](https://www.markdownguide.org/basic-syntax/)

- [Git Documentation](https://git-scm.com/doc)



## Conclusion



Learning PowerShell has helped me understand how much work can be accomplished through automation.



As I continue studying cybersecurity, I want to improve my ability to write scripts that are not only functional but also secure and easy to understand.



For me, the goal is not simply to memorize commands. It is to understand **why they work**, *when to use them*, and how they can help solve real security problems.



---



**Author:** Jamal Rattan



**Course:** MS PowerShell Scripting



**Project:** Lab 4 - Markdown and Working with Excel



