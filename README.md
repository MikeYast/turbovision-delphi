# Turbo Vision for Delphi

This project is a port of Turbo Vision to Delphi. It brings the classic Borland console CUA library to the Delphi Win32 environment, incorporating elements from Virtual Pascal, Free Pascal, and Ilfak Guilfanov's C++ port of Turbo Vision.

## Bugs and Features
1. Save/restore operations from streams do not always work correctly.
2. Collection iterators like `ForEach` and `ForThat` should be invoked as `ForEach(LocalAddr(@Local_Method))`, based on an idea by Max Rusov.
3. On Windows NT/2000, application termination is managed via the hooked event `CTRL_CLOSE_EVENT`.
4. Vertical scrolling with the mouse in `FileViewer` may cause the application to hang.
5. The library has been tested with Delphi 5 and 6; however, for Delphi 6, the `$J+` compiler switch is required.
