# hcipcb21

KiCAD library with custom parts for [CMSC 23230/33230: Engineering Interactive Electronics onto Printed Circuit Boards](http://hcipcb21.plopes.org/) at the University of Chicago (Spring 2021)

## Setup

1. Clone this repository:

```
git clone https://github.com/humancomputerintegration/hcipcb21.git
```

2. In the main window of KiCAD, go to **Preferences > Manage Symbol Libraries > Global Libraries tab**
3. Click **Add existing library to table** (folder icon near the bottom)
4. Select **`hcipcb21.lib`** from the cloned repository. Click Ok and the symbol library is added!
5. In the main window of KiCAD, go to **Preferences > Manage Footprint Libraries > Global Libraries tab**
6. Click **Add existing library to table** (same icon as with Symbol Libraries)
7. Select the **`hcipcb.pretty` folder** from the cloned repository. Click Ok and the footprint library is added!
8. In the main window of KiCAD, go to **Preferences > Configure Paths**
9. **Create a new environmental variable** (+ button on bottom-left) with the **name `HCIPCB_3D`** and **path as the `hcipcb21/3D` directory** (e.g. `/Users/spencerng/hcipcb21/3D`). This helps load the 3D models for footprints.

## Verifying set up

1. **Open a new schematic** (`.sch`) file or re-open an existing one
2. **Add a new symbol** (Place > Place Symbol > click on schematic)
3. You should see **hcipcb21** as a new category. **Place the C21377** onto the schematic. This is the USB connector we'll be using.
4. Go to **Tools > Update PCB from Schematic**, and place the C21377 footprint onto the board.
5. Ensure the 3D model for the USB connector is loaded by going to **View > 3D Viewer**

## Questions?

Email us at the helpdesk (email linked in the class wiki)!
