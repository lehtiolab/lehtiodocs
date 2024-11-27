# Kantele documentation

Please add stuff where you need / like

## File uploads
Files are uploaded from the instrument folder `D:\outbox` to the system, using a filetransfer script in `Desktop\filetransfer\transfer.bat`.
In a column of the acquisition list, you can specify if the file needs to be added to a dataset, or QC immediately:

- Thermo: SampleID
- Bruker: SampleComment

File transfer follows this procedure:
- Start the transfer script. NB: Thermo instruments, the script needs to `Run as administrator`.
- Set the output of the acquisition to `D:\outbox` (not for blanks etc)
- In the SampleID / SampleComment column, write a dataset ID (number) or `QC` if applicable
- Start acquiring
- Transfer script will automatically pick up files that are finished.
- Report bugs :(

If the transfer script is not running, you can start it mid- or post-acquisition.
