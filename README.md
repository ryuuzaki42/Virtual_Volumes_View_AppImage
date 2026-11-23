
# Virtual_Volumes_View_AppImage

 - Virtual Volumes View + Wine

Catalog the content of removable volumes like CD and DVD disks for off-line searching. Folders and files can also be arranged in a single, virtual file system. Each folder of this virtual file system can contain files from many disks

https://sourceforge.net/projects/vvvapp/

## Repository: https://github.com/ryuuzaki42/Virtual_Volumes_View_AppImage
    Virtual Volumes View: 1.5

---
## Using Wine in AppImage from https://github.com/mmtrt/WINE_AppImage - Stable
### Change made:

#### Remove 32 bits
    cd opt/wine-stable/lib/wine/
    rm -r i386-windows/

#### Disable core fonts download/instal
    ... WINEDLLOVERRIDES="mscoree=d;mshtml=d" ...

#### Prefix in RAM - zero disk footprint
    folder_name_RAM="Deffy_AppImage_$(date +%d_%m_%Y)"
    mkdir -p /dev/shm/$folder_name_RAM/
    ... WINEPREFIX=/dev/shm/$folder_name_RAM ...
    rm -r /dev/shm/$folder_name_RAM/

---
https://sourceforge.net/projects/vvvapp/files/VVV/
