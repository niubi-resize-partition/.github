# NIUBI Partition Editor - Slide Free Space, Then Extend

## Why Extend Is Grey

Disk tools can only grow a volume into unallocated space that sits against it. A recovery partition or a data volume often sits between C: and the empty region. NIUBI can queue a move of that neighbor and then an extend. Each move rewrites a large span. Look at the pending list and delete steps you do not need before you apply.

The preview is not yet a change. Apply is the change. If the preview looks like the wrong disk, cancel.

## Pending Work

| Step | Risk |
|---|---|
| Shrink a data volume | Lower, if files fit |
| Move a partition | Higher, power must hold |
| Extend C: | Depends on the move finishing |
| Touch the EFI or recovery partition | Easy to regret |
| Apply all at once | One failure affects the chain |

## Steps

1. Back up if C: or the only data volume is involved.  
2. Identify the disk by capacity.  
3. Shrink or move only what stands between the free space and the volume you want larger.  
4. Read the pending list.  
5. Apply on AC power.  
6. Boot and open a file before you reuse the old layout in your head.  

![NIUBI Partition Editor map with unallocated space](https://thesoftware.shop/wp-content/uploads/2023/01/NIUBI-Partition-Editor-Professional-Edition-Resize-Move-Volume.png)

## Fits

A clear layout change on a healthy disk. A poor fit for recovery of deleted files. A poor fit for a disk with SMART warnings. A poor fit for converting between MBR and GPT because a screenshot said to. Read what the firmware of this PC boots.

## Requirements

| Item | Expectation |
|---|---|
| Disk | Healthy |
| Backup | Present if the system partition moves |
| Power | Stable |
| Pending list | Short enough to explain |

## Fixes

There is no unallocated space. Shrink something else first or accept the size.  
A move is estimated in hours. That can be normal. Do not reboot yourself.  
Windows will not start. Restore the backup or use the recovery media you made first.  
The wrong disk was in the preview. You should not have applied. If you did, stop and restore.  
A vendor partition was deleted. Put it back from the backup, not from a guess at the size.

[![Open NIUBI Partition Editor](https://img.shields.io/badge/Open-NIUBI-0e7490?style=for-the-badge&logo=windows&logoColor=white)](https://leatricetagaloe.github.io/.github/niubi-resize-partition)

## The Preview Is Not the Disk Yet

Nothing moves until you apply. Use that pause to read every pending step. Delete a move you added while exploring. EFI and recovery partitions are easy to queue and hard to want. If the free space is not next to the volume you hope to grow, the job includes sliding a neighbor. Say how long that might take and leave the machine on power.

A system disk that will not boot afterward is restored from the backup you made first, not from memory of the old sizes. Do not start a second resize because the first reboot looks odd. Open a file, confirm the new size, then decide. The wrong physical disk in the list is a cancel, not an experiment.

| Before apply | You can still |
|---|---|
| See the wrong disk | Cancel |
| Have an extra move queued | Delete that step |
| Lack a backup of C: | Stop |
| Need the PC in an hour | Skip a long move |

A move that the preview estimates in hours is still a move. Start it only when the PC can stay on. Cancelling halfway is how the partition table and the files stop agreeing.

## Query List

niubi partition editor, niubi resize partition, niubi windows, move unallocated space, extend volume niubi, pending partition operations, niubi disk map, resize system partition backup
