skip:
	dynapi\SDL_dynapi.c
	audio\winmm\SDL_winmm.c
	audio\wasapi\SDL_wasapi.c
	audio\wasapi\SDL_wasapi_win32.c
	audio\wasapi\SDL_wasapi_winrt.cpp
	render\opengles2\sdl_render_gles2.c
	render\opengles2\sdl_shaders_gles2.c
src\render\direct3d
src\render\direct3d11
joystick\hidapi
src\audio\directsound\sdl_directsound.c

-----------

#if _MSC_VER > 1200
        messageboxdata = (const SDL_MessageBoxData *)GetWindowLongPtr(hDlg, GWLP_USERDATA);
        
------------

int
WIN_InitModes(_THIS)
{
    SDL_VideoDisplay display;
	SDL_DisplayMode mode;

    SDL_zero(display);
	SDL_zero(mode);

    display.name = NULL;
    display.desktop_mode = mode;
    display.current_mode = mode;
    display.driverdata = NULL;
    SDL_AddVideoDisplay(&display);

    return 0;
}

---------------
