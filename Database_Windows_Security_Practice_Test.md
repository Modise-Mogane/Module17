# Database / Windows Security — Practice Test

## Part A: Multiple Choice — 30 Questions

**1.** Which Windows editions include the Local Group Policy and Local Security Policy editors?

a) Home only  
b) Home & Pro  
c) Business/Pro editions  
d) All editions  

**2.** Which component is commonly required for BitLocker computer authentication?

a) HSM  
b) TPM  
c) UEFI Secure Boot  
d) Intel TXT  

**3.** Which of the following is required for Encrypting File System (EFS)?

a) FAT32 volume  
b) NTFS and Business/Pro edition  
c) Domain join  
d) BitLocker enabled first  

**4.** A folder is marked for EFS encryption. What happens to new files created inside that folder?

a) They remain unchanged  
b) They are encrypted only if manually selected  
c) They are encrypted automatically  
d) They are compressed instead  

**5.** Which type of Windows share is hidden by default and commonly accessed by administrators?

a) Public$  
b) Temp$  
c) Administrative shares such as ADMIN$ and C$  
d) Everyone$  

**6.** Where would you configure the policy that requires users to log on using a smart card?

a) Computer Configuration → Windows Settings → Security Settings → Local Policies → Security Options  
b) Computer Configuration → Windows Settings → Security Settings → Biometrics  
c) User Configuration → Windows Settings → Logon  
d) Computer Configuration → Administrative Templates → System → Logon  

**7.** Which statement about share permissions and NTFS permissions is most accurate?

a) Share permissions apply to local users  
b) NTFS permissions work on NTFS volumes for local and network access  
c) Only share permissions matter when accessing files over a network  
d) NTFS permissions apply to folders but never to files  

**8.** When accessing a shared folder across a network, effective access is generally determined by:

a) The least restrictive of the share and NTFS permissions  
b) The most restrictive of the share and NTFS permissions  
c) Share permissions only  
d) NTFS permissions only  

**9.** Which command reports the resultant Group Policy information for the current user/computer?

a) rsop.msc  
b) gpresult /r  
c) whoami /priv  
d) lusrmgr.msc  

**10.** What does mapping a network drive do?

a) Makes the remote share appear as a drive letter on the client  
b) Creates a printer port  
c) Creates a DFS namespace  
d) Creates a new partition on the server  

**11.** Which sign-in methods can Windows Hello support?

a) Face, iris, fingerprint, and PIN  
b) Password only  
c) Smart card only  
d) TPM only  

**12.** The Local Users and Groups console (`lusrmgr.msc`) is typically available in which Windows editions?

a) Home  
b) Education  
c) Pro/Business editions  
d) Any edition with S mode  

**13.** A firmware “drive lock password” primarily protects:

a) CPU microcode  
b) The hard drive itself, including if the drive is removed from the computer  
c) UEFI variables  
d) Network adapters  

**14.** Which statement about the Windows Guests group is correct?

a) Members have full administrative rights  
b) Members have limited privileges and their temporary profile is deleted at logoff  
c) Membership requires the computer to be joined to a domain  
d) Members can manage Group Policy Objects  

**15.** What is the primary reason the Power Users group remains present in modern Windows versions?

a) To provide day-to-day administrative privileges  
b) For backward compatibility  
c) To enforce domain Group Policies  
d) To provide EFS key escrow  

**16.** In Active Directory, where are policy settings contained?

a) GPOs  
b) OUs  
c) Sites  
d) Domains  

**17.** In normal Group Policy processing, which level is generally applied last?

a) Local  
b) Site  
c) Domain  
d) OU  

**18.** Where is the most appropriate location for data that all users on a standalone Windows PC should be able to share?

a) `C:\Users\Public`  
b) `C:\Windows\System32`  
c) `C:\Program Files`  
d) `C:\Temp`  

**19.** How can the Everyone group be removed from a shared folder's share permissions?

a) Use Disk Cleanup  
b) Advanced Sharing → Permissions → Remove  
c) NTFS Properties → Auditing  
d) BitLocker Control Panel  

**20.** How can you hide a shared folder while keeping it shared?

a) Add a `$` suffix to the share name  
b) Encrypt it with EFS only  
c) Disable NTFS  
d) Use DFS only  

**21.** Which command displays the group memberships of the currently signed-in account?

a) `whoami /groups`  
b) `gpedit.msc`  
c) `secpol.msc`  
d) `compmgmt.msc`  

**22.** What does BitLocker To Go primarily encrypt?

a) System RAM  
b) USB flash/removable drives  
c) BIOS firmware  
d) CPU cache  

**23.** When a folder is moved to a different volume, what typically happens to its permissions?

a) The original ACLs are always retained  
b) The permissions become read-only  
c) The folder inherits permissions from the destination's parent  
d) All permissions are removed  

**24.** For least-privilege permission management, permissions should generally be assigned to:

a) Individual user accounts  
b) Groups  
c) Computers  
d) Sites  

**25.** A user cannot access a mapped network share. What is an appropriate first troubleshooting step?

a) Check network connectivity and credentials, then remap if necessary  
b) Factory reset the computer  
c) Disable the firewall  
d) Delete the user profile  

**26.** Which Windows Reset option removes applications and settings while keeping the user's personal files?

a) Keep nothing  
b) Keep personal files  
c) Restore OEM apps only  
d) Repair install  

**27.** What does Startup Repair primarily attempt to repair?

a) User profiles  
b) Critical Windows system files, services, and drivers  
c) Office activation  
d) Printer queues  

**28.** Where does Startup Repair write its main diagnostic log?

a) `%SystemRoot%\INF`  
b) `C:\Windows\System32\LogFiles\SRT\SRTTrail.txt`  
c) `C:\Windows\Panther`  
d) `%TEMP%`  

**29.** Which Windows Advanced Startup option is specifically used to roll back a recent Windows Update?

a) System Restore  
b) Uninstall Updates  
c) System Image Recovery  
d) Startup Settings  

**30.** Which command can restart Windows and launch Windows Recovery Environment from a running operating system?

a) `shutdown /r /o`  
b) `sfc /scannow`  
c) `chkdsk /r`  
d) `dism /online /cleanup-image`  

---

# Part B: Match Column A with Column B — 20 Questions

## Instructions

Match each term in **Column A** with the **most appropriate description in Column B**.

## Column A

| No. | Term |
|---:|---|
| 1 | TPM |
| 2 | BitLocker To Go |
| 3 | EFS |
| 4 | Windows Hello |
| 5 | `gpedit.msc` |
| 6 | `secpol.msc` |
| 7 | `lusrmgr.msc` |
| 8 | `gpresult /r` |
| 9 | `whoami /groups` |
| 10 | Administrative shares |
| 11 | Mapped drive |
| 12 | NTFS permissions |
| 13 | Share permissions |
| 14 | Everyone group |
| 15 | Guests group |
| 16 | OU (Organizational Unit) |
| 17 | GPO |
| 18 | Policy precedence |
| 19 | Public folder |
| 20 | Advanced Sharing |

## Column B

**A.** A location where all users on a computer can share data.

**B.** A hardware chip commonly used to securely store/protect a BitLocker startup key and assist with computer authentication.

**C.** A Windows feature that encrypts individual files and folders on NTFS volumes.

**D.** A client-side drive letter that points to a shared folder located on another computer.

**E.** A command that displays the group memberships of the current user.

**F.** A Windows sign-in feature supporting methods such as facial recognition, iris recognition, fingerprint recognition, and PIN.

**G.** Permissions that apply to files and folders on NTFS volumes and can affect both local and network access.

**H.** The Local Group Policy Editor.

**I.** A group that provides limited privileges and is intended for temporary or restricted users.

**J.** A graphical interface used to configure sharing and manage share permissions, including adding or removing users and groups.

**K.** A feature that encrypts removable storage devices such as USB flash drives.

**L.** The Local Security Policy Editor, which provides a subset of Local Group Policy security settings.

**M.** A container in Active Directory used to organize users and computers and to scope Group Policy.

**N.** Permissions that apply specifically when a folder is accessed through a network share.

**O.** A command used to report the resultant Group Policy information applied to a user or computer.

**P.** A collection of policy settings stored in Active Directory and applied to users and/or computers.

**Q.** Hidden default shares such as `ADMIN$` and `C$` that are commonly intended for administrative access.

**R.** A group that includes Authenticated Users and Guest accounts.

**S.** The order in which Windows Group Policies are processed: Local, Site, Domain, then OU.

**T.** The Local Users and Groups management console, typically available in Pro/Business editions.
