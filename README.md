pip install kivy
from kivy.app import App
from kivy.uix.label import Label

class MyGame(App):
    def build(self):
        return Label(text='Hello, Kivy!')

if __name__ == '__main__':
    MyGame().run()
pip install buildozer
[app]

# (str) Title of your application
title = My Kivy Game

# (str) Package name
package.name = mykivygame

# (str) Package domain (reverse domain style)
package.domain = org.example

# (str) Source code where the main.py is located
source.dir = .

# (str) Source code where the main.py is located
source.include_exts = py,png,jpg,kv,atlas

[buildozer]

# (list) List of source files to include
source.include_exts = py,png,jpg,kv,atlas

# (list) List of source files to exclude
source.exclude_exts = spec

# (list) List of directories to include
source.include_dirs = 

# (list) List of directories to exclude
source.exclude_dirs = 

# (list) List of the source files to include (let empty to include all the files)
source.include_patterns = 

# (list) List of the source files to exclude (let empty to not exclude anything)
source.exclude_patterns = 

# (list) List of the framework directories (if any)
frameworks = kivy

# (str) Custom source folders for requirements (Separate folders with a comma)
requirements.source.kivy = ../../kivy

# (list) List of all the modules to include by default (let empty to include all)
requirements = python3,kivy

# (str) Custom source folders for requirements (Separate folders with a comma)
requirements.source.kivy = ../../kivy

# (list) Application requirements
# comma separated e.g. requirements = sqlite3,kivy
requirements = kivy

# (str) Presplash of the application
presplash.filename = %(source.dir)/data/presplash.png

# (str) Icon of the application
icon.filename = %(source.dir)/data/icon.png

# (str) Supported orientation (one of landscape, sensorLandscape, portrait or all)
orientation = portrait

# (bool) Indicate if the application should be fullscreen or not
fullscreen = 1

# (list) Permissions
android.permissions = INTERNET
buildozer android debug deploy run

