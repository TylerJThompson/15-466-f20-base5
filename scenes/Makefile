#This makefile for Windows was originally made by Dominic Calkosz and made available in the class Discord.
#I did not write this makefile originally, I edited it for scenes besides hexapod and to run export-walkmeshes.py

all : \
    ../dist/phone-bank.pnct \
    ../dist/phone-bank.scene \
    ../dist/phone-bank.w \

../dist/phone-bank.scene : phone-bank.blend export-scene.py
    "E:\Program Files\Blender Foundation\Blender 2.90\blender.exe" --background --python export-scene.py -- "phone-bank.blend:Platforms" "../dist/phone-bank.scene"

../dist/phone-bank.pnct : phone-bank.blend export-meshes.py
    "E:\Program Files\Blender Foundation\Blender 2.90\blender.exe" --background --python export-meshes.py -- "phone-bank.blend:Platforms" "../dist/phone-bank.pnct"

../dist/phone-bank.w : phone-bank.blend export-walkmeshes.py
    "E:\Program Files\Blender Foundation\Blender 2.90\blender.exe" --background --python export-walkmeshes.py -- "phone-bank.blend:WalkMeshes" "../dist/phone-bank.w"