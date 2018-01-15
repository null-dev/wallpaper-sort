# wallpaper-sort
A bash script to categorize images as 'phone' or 'desktop' wallpapers based on their dimensions.

## Behavior
Images that are wider than they are tall are classified as desktop wallpapers.

Images that are taller than they are wide are classified as phone wallpapers.

Images that are square are ignored.

The classified images are then moved into their separate directories (directories specified as arguments and are created if missing).

### Usage
```
Usage: ./wallpaper-sort <DESKTOP_DIR> <PHONE_DIR> [FILE]...
	DESKTOP_DIR: The location to move the desktop wallpapers to
	PHONE_DIR: The location to move the phone wallpapers to
	FILE: The images to sort
```

#### Sample usage
To classify all images in a directory, moving desktop wallpapers into a directory called "Desktop" and phone wallpapers into a directory called "Phone":
```
wallpaper-sort Desktop Phone *
```
