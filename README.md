# CBT434
Converted to GitHub via [cbt2git](https://github.com/wizardofzos/cbt2git)

This is still a work in progress. GitHub repos will be deleted and created during this period...

```
//***FILE 434 is from Mark Zelden and contains his collection       *   FILE 434
//*           of MVS utilities.                                     *   FILE 434
//*                                                                 *   FILE 434
//*   Questions: Please email Mark Zelden -  mark@mzelden.com       *   FILE 434
//*                                                                 *   FILE 434
//*   Last Updated:  January 11, 2025                               *   FILE 434
//*                                                                 *   FILE 434
//*   Mark's MVS Utilities is also available on the web:            *   FILE 434
//*      http://www.mzelden.com/mvsutil.html                        *   FILE 434
//*                                                                 *   FILE 434
//*                                                                 *   FILE 434
//* Sample JOBs / Documentation                                     *   FILE 434
//* --------------------------------------------------------------- *   FILE 434
//* $$$$READ  - Disclaimer                                          *   FILE 434
//* $$$INDEX  - Index of all members                                *   FILE 434
//* $$CHANGE  - CBT File 434 change log                             *   FILE 434
//* $$INSTAL  - General installation documentation for this file    *   FILE 434
//* $ONEPAK   - Doc for using DFSMSdss instead of FDRCOPY for       *   FILE 434
//*             ONEPAK / TWOPAK jobs.                               *   FILE 434
//* $ROOTSHR  - Doc for setting up a shared UNIX root file          *   FILE 434
//* $RXINTRO  - Doc to download and use RXINTRO member              *   FILE 434
//* $SNGLTSO  - Doc for using the same TSO USERID in a shared       *   FILE 434
//*             environment.                                        *   FILE 434
//* $WLMMONO  - Doc for setting up WLM in a MONOPLEX                *   FILE 434
//* CLONERES  - Sample jobstream to clone a two volume sysres set   *   FILE 434
//*             and SMP/E target zones.                             *   FILE 434
//* CLONERSO  - Old version of CLONERES                             *   FILE 434
//* ISPDFLTS  - ISPF defaults source update needed for single TSO   *   FILE 434
//*             USERID (described in $SNGLTSO).                     *   FILE 434
//* ISPEX16   - ISPXDT and ISPF exit 16 source needed for single    *   FILE 434
//*             TSO USERID (described in $SNGLTSO).                 *   FILE 434
//* ONEPAKZ3  - Sample jobstream to build a one pack "rescue"       *   FILE 434
//*             system from a z/OS 1.3 driving system.              *   FILE 434
//* ONEPAKZ6  - Sample jobstream to build a one pack "rescue"       *   FILE 434
//*             system from a z/OS 1.6 driving system.              *   FILE 434
//* ONEPAKZ8  - Sample jobstream to build a one pack "rescue"       *   FILE 434
//*             system from a z/OS 1.7 - z/OS 1.11 driving system.  *   FILE 434
//* ONEPAKZD  - Sample jobstream to build a one pack "rescue"       *   FILE 434
//*             system from a z/OS 1.12 - z/OS 1.13 driving system. *   FILE 434
//* ONEPAK21  - Sample jobstream to build a one pack "rescue"       *   FILE 434
//*             system from a z/OS 2.1 driving system.              *   FILE 434
//* ONEPAK22  - Sample jobstream to build a one pack "rescue"       *   FILE 434
//*             system from a z/OS 2.2 or 2.3 driving system.       *   FILE 434
//* ONEPAK43  - Sample jobstream to build a one pack "rescue"       *   FILE 434
//*             system (created for ESA 4.3, but is still a good    *   FILE 434
//*             sample of the required steps).                      *   FILE 434
//* RXINTRO   - "Introduction to TSO/E REXX" Word document          *   FILE 434
//* SMPBLD1   - Job to build an SMP/E environment from scratch.     *   FILE 434
//*             All VSAM SMP/E zones are created within the same    *   FILE 434
//*             physical VSAM data set.                             *   FILE 434
//* SMPBLD2   - Job to build an SMP/E environment from scratch.     *   FILE 434
//*             The VSAM SMP/E zones are created as separate        *   FILE 434
//*             physical VSAM data sets.                            *   FILE 434
//* SMPBLD3   - Job to build a new SMP/E target zone, dlib zone,    *   FILE 434
//*             and other required SMP/E data sets into an          *   FILE 434
//*             existing global zone.                               *   FILE 434
//* SMPDELF   - Sample job to delete a FMID from a set of SMP/E     *   FILE 434
//*             zones and libraries.                                *   FILE 434
//* TWOPAKZ3  - Sample jobstream to build a two pack "rescue"       *   FILE 434
//*             system from a z/OS 1.3 driving system. Same as      *   FILE 434
//*             ONEPAKZ3 but also includes Unix System Services,    *   FILE 434
//*             TCP/IP, and ISHELL.                                 *   FILE 434
//* TWOPAKZ6  - Sample jobstream to build a two pack "rescue"       *   FILE 434
//*             system from a z/OS 1.6 driving system. Same as      *   FILE 434
//*             ONEPAKZ6 but also includes Unix System Services,    *   FILE 434
//*             TCP/IP, and ISHELL.                                 *   FILE 434
//* TWOPAKZ8  - Sample jobstream to build a two pack "rescue"       *   FILE 434
//*             system from a z/OS 1.7 - z/OS 1.11 driving system.  *   FILE 434
//*             Same as ONEPAKZ8 but also includes Unix System      *   FILE 434
//*             Services, TCP/IP, and ISHELL.                       *   FILE 434
//* TWOPAKZD  - Sample jobstream to build a two pack "rescue"       *   FILE 434
//*             system from a z/OS 1.12 - z/OS 1.13 driving system. *   FILE 434
//*             Same as ONEPAKZD but also includes Unix System      *   FILE 434
//*             Services, TCP/IP, and ISHELL.                       *   FILE 434
//* TWOPAK21  - Sample jobstream to build a two pack "rescue"       *   FILE 434
//*             system from a z/OS 2.1 driving system.              *   FILE 434
//*             Same as ONEPAK21 but also includes Unix System      *   FILE 434
//*             Services, TCP/IP, and ISHELL.                       *   FILE 434
//* TWOPAK22  - Sample jobstream to build a two pack "rescue"       *   FILE 434
//*             system from a z/OS 2.2 or 2.3 driving system.       *   FILE 434
//*             Same as ONEPAK22 but also includes Unix System      *   FILE 434
//*             Services, TCP/IP, and ISHELL.                       *   FILE 434
//* UMJES01   - JES2 source update needed for single TSO USERID     *   FILE 434
//*             (OS/390 R10 & z/OS R1 - described in $SNGLTSO).     *   FILE 434
//* UMJES012  - JES2 source update needed for single TSO USERID     *   FILE 434
//*             (z/OS R2 and above - described in $SNGLTSO).        *   FILE 434
//* UMJES01O  - JES2 source update needed for single TSO USERID     *   FILE 434
//*             (prior to OS/390 R10 - described in $SNGLTSO).      *   FILE 434
//* UMJES06   - JES3 source update needed for single TSO USERID     *   FILE 434
//*             (described in $SNGLTSO).                            *   FILE 434
//*                                                                 *   FILE 434
//*                                                                 *   FILE 434
//* CLISTS / Edit Macros / Programs                                 *   FILE 434
//* --------------------------------------------------------------- *   FILE 434
//* ACBCHECK  - ASM PGM to check if a VTAM APPLID is available      *   FILE 434
//* AMBCLIST  - CLIST to invoke interactive AMBLIST with panel I/P  *   FILE 434
//* APFVER    - REXX exec to verify APF list                        *   FILE 434
//* ASIDLIST  - ASM PGM to list ASIDs & MAXUSER/RSVSTRT/RSVNONR     *   FILE 434
//* ASIDLRX   - REXX PGM to list ASIDs & MAXUSER/RSVSTRT/RSVNONR    *   FILE 434
//* BLKCLIST  - CLIST to invoke BLKDISK command with panel input    *   FILE 434
//* CAT       - REXX exec to invoke CATSRCH via CATSRCHP panel      *   FILE 434
//* CATSRCH   - REXX exec to invoke Catalog Search Interface (CSI)  *   FILE 434
//* CMD34     - REXX exec to process commands against a DSLIST      *   FILE 434
//* COLADD    - Edit macro to add numbers from a column range       *   FILE 434
//* COLUTIL   - Edit macro to manipulate columns                    *   FILE 434
//* DB        - Edit macro to delete lines from the cursor line     *   FILE 434
//*             to the bottom line                                  *   FILE 434
//* DELDUPS   - Edit macro to delete duplicate lines                *   FILE 434
//* DELDUPS2  - REXX duplicate record deletion program              *   FILE 434
//* DELNX     - Edit macro to delete all of a certain string        *   FILE 434
//* DELX      - Edit macro to delete everything but a certain       *   FILE 434
//*             string                                              *   FILE 434
//* DSLISTSV  - Quick ISPF save of data set names similar to        *   FILE 434
//*             ISPF 3.4                                            *   FILE 434
//* DT        - Edit macro to delete lines from the cursor line     *   FILE 434
//*             to the top line                                     *   FILE 434
//* EDMACALL  - REXX exec to run an edit macro against every        *   FILE 434
//*             member of a PDS.                                    *   FILE 434
//* EXCL      - Edit macro to exclude all of certain string         *   FILE 434
//* FILL      - Edit macro to fill columns with a character         *   FILE 434
//* FINDMOD   - REXX exec (command) to find what library(s) a       *   FILE 434
//*             module is in                                        *   FILE 434
//* FINDASYS  - Sample search list for FINDMOD CLIST                *   FILE 434
//* FVE       - REXX exec (command) - Fast View/Edit of DSNs        *   FILE 434
//* HLISTB    - REXX exec to browse o/p of HLIST DA BCDS (BACKUP)   *   FILE 434
//* HLISTBL   - REXX exec to browse o/p of HLIST DA LEVEL BCDS      *   FILE 434
//* HLISTM    - REXX exec to browse o/p of HLIST DA MCDS (MIGRATE)  *   FILE 434
//* HLISTML   - REXX exec to browse o/p of HLIST DA LEVEL MCDS      *   FILE 434
//* INCL      - Edit macro to include all of a certain string       *   FILE 434
//* INDIRECR  - REXX exec to create IDCAMS control cards for        *   FILE 434
//*             indirectly catalogging a list of data set names     *   FILE 434
//* INSLINE   - Edit macro to insert a string after or before lines *   FILE 434
//* IPLHIST   - REXX exec to create a history of IPLs. This exec    *   FILE 434
//*             calls IPLINFO as a function.                        *   FILE 434
//* IPLINFO   - REXX exec to show various system information        *   FILE 434
//* JOBCHECK  - ASM PGM to find if a JOB is active on the system    *   FILE 434
//* JOBCHKRX  - REXX PGM to find if a JOB is active on the system   *   FILE 434
//* ISPCMDSA  - CLIST to add temporary cmds to ISPF command table   *   FILE 434
//* KEYSWAP   - REXX exec to swap PFKEYS 1-12 with PFKEYS 13-24     *   FILE 434
//* LASTIPL   - REXX exec to display last (latest) IPLHIST info     *   FILE 434
//* LINEMAC   - REXX exec - used with Doug Nadel's / IBM's LMAC PGM *   FILE 434
//* LINETBL   - Sample ISPF table to use with ISPF line edit macros *   FILE 434
//* LMPREXX   - REXX exec to help manage CA LMP KEYS                *   FILE 434
//* LOGRREXX  - REXX program to build logstream DELETE/DEFINE cards *   FILE 434
//*             using the output from IXCMIAPU LIST LOGSTREAM.      *   FILE 434
//* LNKVER    - REXX exec to verify LNKLST syntax and libs          *   FILE 434
//* LPROG     - REXX exec - displays LNKLST, LPA list, & APF list   *   FILE 434
//* MEMLSTSV  - Quick ISPF save of member stats. Similar to "SAVE"  *   FILE 434
//*             command from a data set member list.                *   FILE 434
//* PREFIX    - Edit macro to add a prefix to the front of a line   *   FILE 434
//* PREFIX2   - Edit macro to add a prefix to the front of a line   *   FILE 434
//* RACFUDEL  - REXX program to remove obsolete RACF users          *   FILE 434
//* RDATE     - REXX date conversion routine                        *   FILE 434
//* RDATEF    - REXX function version of RDATE                      *   FILE 434
//* REXXMEM   - REXX program to browse memory in "dump" format      *   FILE 434
//* REXXSCAN  - REXX program to scan an input file for string(s)    *   FILE 434
//* REXXSTOR  - REXX exec to show virtual storage usage of invoker  *   FILE 434
//* REXXSTOJ  - Sample JCL to run REXXSTOR in batch                 *   FILE 434
//* RXSMF30   - REXX program to read SMF 30 records and produce     *   FILE 434
//*             produce a job accounting report.                    *   FILE 434
//* RXSTOR64  - REXX exec to show 64-bit MEMLIMIT and storage use   *   FILE 434
//* SDSF@DR   - REXX program to that uses the SDSF REXX environment *   FILE 434
//*             to copy output from the spool into data sets.       *   FILE 434
//* SDSFPRT   - REXX program to that uses the SDSF REXX environment *   FILE 434
//*             to take all or selected output from the spool and   *   FILE 434
//*             copy it to a PDS via SDSF "PRINT" commands.         *   FILE 434
//* SUFFIX    - Edit macro to add a suffix to the end of a line     *   FILE 434
//* SW        - Edit macro to switch from VIEW to EDIT or visa versa*   FILE 434
//* TAPESTAK  - REXX tape stacking program (works with CA-1)        *   FILE 434
//* TSOB      - REXX exec (command) to BROWSE o/p of any TSO cmd    *   FILE 434
//* TSOE      - REXX exec (command) to EDIT o/p of any TSO cmd      *   FILE 434
//* TSOR      - REXX exec (command) to REVIEW o/p of any TSO cmd    *   FILE 434
//* TSOV      - REXX exec (command) to VIEW o/p of any TSO cmd      *   FILE 434
//* VTOCTOT   - REXX program to summarize VTOC cmd output by HLQ    *   FILE 434
//* XBROWSE   - REXX (command) to browse any dataset                *   FILE 434
//* XDSLIST   - REXX (command) to display a data set list (ISPF 3.4)*   FILE 434
//* XEDIT     - REXX (command) to edit any dataset                  *   FILE 434
//* XEF       - REXX exec to start eXtended Editor Facility dialog  *   FILE 434
//* XEFLIBD   - REXX exec to start eXtended Editor Facility dialog  *   FILE 434
//* XEFCLIST  - eXtended Editor Facility mainline code              *   FILE 434
//* XLISTC    - REXX (command) to LISTCAT ALL any dataset           *   FILE 434
//* XMEMLIST  - CLIST (command) to bring up member list on any DSN  *   FILE 434
//* XVIEW     - REXX (command) to view any dataset                  *   FILE 434
//* ZBROWSE   - Edit macro to browse dataset that the cursor is on  *   FILE 434
//* ZEDIT     - Edit macro to edit dataset that the cursor is on    *   FILE 434
//* ZVIEW     - Edit macro to view dataset that the cursor is on    *   FILE 434
//*                                                                 *   FILE 434
//*                                                                 *   FILE 434
//* ISPF Panels                                                     *   FILE 434
//* --------------------------------------------------------------- *   FILE 434
//* AMBPANEL  - Interactive AMBLIST panel for AMBCLIST              *   FILE 434
//* BLKPANEL  - Interactive BLKDISK panel for BLKCLIST              *   FILE 434
//* CATSRCHP  - Optional panel for invoking CATSRCH REXX exec       *   FILE 434
//* XEFMENU   - eXtended Editor Facility Main Menu                  *   FILE 434
//* XEFMENUB  - eXtended Editor Facility Main Menu (optional)       *   FILE 434
//* XEFHELP   - eXtended Editor Facility Help Panel #1              *   FILE 434
//* XEFHELP2  - eXtended Editor Facility Help Panel #2              *   FILE 434
//* XEFHELP3  - eXtended Editor Facility Help Panel #3              *   FILE 434
//* XEFHELP4  - eXtended Editor Facility Help Panel #4              *   FILE 434
//* XEFINF    - eXtended Editor Facility Dataset Info Panel-SEQ     *   FILE 434
//* XEFINFD   - eXtended Editor Facility Dataset Info Panel-PDS     *   FILE 434
//* XEFINFE   - eXtended Editor Facility Dataset Info Panel-PDSE    *   FILE 434
//* XEFINFP   - eXtended Editor Facility Dataset Info Panel-PDS SMS *   FILE 434
//* XEFINFS   - eXtended Editor Facility Dataset Info Panel-SEQ SMS *   FILE 434
//*                                                                 *   FILE 434
//*                                                                 *   FILE 434
//* ISPF MESSAGEs                                                   *   FILE 434
//* --------------------------------------------------------------- *   FILE 434
//* XEF00     - eXtended Editor Facility Messages                   *   FILE 434
//*                                                                 *   FILE 434
//*                                                                 *   FILE 434
//* Miscellaneous                                                   *   FILE 434
//* --------------------------------------------------------------- *   FILE 434
//* XEF62     - XEF V6.2 in TSO XMIT format                         *   FILE 434
//*                                                                 *   FILE 434
```
