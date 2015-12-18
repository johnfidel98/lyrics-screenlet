# lyrics-screenlet

Added fix for 
>Traceback (most recent call last):
>  File "/usr/share/screenlets/Lyrics/LyricsScreenlet.py", line 1610, in <module>
>    screenlets.session.create_session(LyricsScreenlet)	
>  File "/usr/lib/pymodules/python2.7/screenlets/session.py", line 480, in create_session
>    session.start()
>  File "/usr/lib/pymodules/python2.7/screenlets/session.py", line 245, in start
>    if self.__load_instances():
>  File "/usr/lib/pymodules/python2.7/screenlets/session.py", line 399, in __load_instances
>    sl = self.create_instance(id=filename[:-4], enable_saving=False)
>  File "/usr/lib/pymodules/python2.7/screenlets/session.py", line 151, in create_instance
>    sl = self.screenlet(id=id, session=self, **keyword_args)
>  File "/usr/share/screenlets/Lyrics/LyricsScreenlet.py", line 307, in __init__
>    self.theme_name = 'default'
>  File "/usr/share/screenlets/Lyrics/LyricsScreenlet.py", line 352, in __setattr__
>    self.onThemeChanged(self.theme)
>  File "/usr/share/screenlets/Lyrics/LyricsScreenlet.py", line 1432, in onThemeChanged
>    self.canvas.setTheme(self.theme)
>  File "/usr/share/screenlets/Lyrics/gui/widget.py", line 172, in setTheme
>    widget.setTheme(self.theme)
>  File "/usr/share/screenlets/Lyrics/gui/cairo_widgets.py", line 137, in setTheme
>    self.updateDimensions()
>  File "/usr/share/screenlets/Lyrics/gui/cairo_widgets.py", line 147, in updateDimensions
>    dimensions = self.theme.get_image_dimensions(self.image)
>  File "/usr/share/screenlets/Lyrics/gui/widget.py", line 71, in get_image_dimensions
>    return self.svgs[name].get_dimension_data()
>AttributeError: 'gtk.gdk.Pixbuf' object has no attribute 'get_dimension_data'
