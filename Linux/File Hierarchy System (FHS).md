
A Guideline that defines the common structure, content, and purpose of directories in Linux distributions.

- **`/`:** The root directory. The starting point of the entire file system.
- **`/root`**: Home directory for root user.
- **`/bin`:** Essential command binaries for all users (e.g., ls, cat, cp).
- **`/sbin`:** System administration binaries (usually only accessible by root).
- **`/etc`:** System-wide configuration files.
- **`/home`:** Home directories for individual users.
- **`/lib`:** Shared libraries required by binaries in `/bin` and `/sbin`.
- **`/usr`:** Read-only user data. Contains applications, documentation, shared libraries, and more.
    - **`/usr/bin`** Non-essential command binaries.
    - **`/usr/local`** Locally installed software, ideal for third-party applications.
- **`/var`:** Variable data like logs, databases, mailboxes, etc.
- **`/tmp`:** Temporary files (often cleared on reboot).
- **`/boot`:** Bootloader files.
- **`/media`**: Mount point for removable media.
- **`/mnt`**: Mount point for temporarily mounted filesystems.
- **`/dev`**: Device files
- **`/opt`:** Optional additional software packages.

 >	**Note:**  Directory Names are case sensitive. `/boot` is different from `/Boot.`
 
 > **Tip:** 
 > Access `/root` from `Computer` in Fs GUI.
 > `Ctrl+L` to see current file path. 
 
 
 
 