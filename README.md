# stl-thumbnailer
Shows thumbnails of STL files in Nautilus file browser. The sources are based on [linux nautilus stl thumbnailer :)](http://www.thingiverse.com/thing:258653)



### Install 

    sudo cp stl_thumb.py /usr/local/bin/
    sudo chmod a+x /usr/local/bin/stl_thumb.py
    sudo cp stl.thumbnailer /usr/share/thumbnailers/
    cp stl.xml ~/.local/share/mime/packages/

After that you should update MIME database by runnig following command and restarting Nautilus by closing all windows or log out and login to the desktop. 

    update-mime-database ~/.local/share/mime/

Now the STL thumbnails should show-up. Else you need to remove thumbnails cache '''rm -rf ~/.cache/thumbnails/*''' and restarting Nautilus again. 

### Thumbnails preview from OpenSCAD files

If you looking for an preview generated from .scad files you could check [OpenSCAD Thumbnailer for Gnome](http://srlm.io/2015/12/15/scad-thumbnailer/) but computing power required for rendering more complicated scad model could be prohibitive to use this approach. 


