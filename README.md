TO INSTALL RUN Installer.py
.______       __    __  .__   __.     _ _ __  .__   __.      _______.___________.    ___       __       __       _______ .______        .______   ____    ____  _ _ 
|   _  \     |  |  |  | |  \ |  |    ( | )  | |  \ |  |     /       |           |   /   \     |  |     |  |     |   ____||   _  \       |   _  \  \   \  /   / ( | )
|  |_)  |    |  |  |  | |   \|  |     V V|  | |   \|  |    |   (----`---|  |----`  /  ^  \    |  |     |  |     |  |__   |  |_)  |      |  |_)  |  \   \/   /   V V 
|      /     |  |  |  | |  . `  |        |  | |  . `  |     \   \       |  |      /  /_\  \   |  |     |  |     |   __|  |      /       |   ___/    \_    _/        
|  |\  \----.|  `--'  | |  |\   |        |  | |  |\   | .----)   |      |  |     /  _____  \  |  `----.|  `----.|  |____ |  |\  \----.__|  |          |  |          
| _| `._____| \______/  |__| \__|        |__| |__| \__| |_______/       |__|    /__/     \__\ |_______||_______||_______|| _| `._____(__) _|          |__|          
                                                                                                                                                                                                                                                                                                                                                                            
BYFRON IS OUT, BUT IM BYPASSING IT LOL

TaaprWare V3
Discord (real exploits here): https://discord.gg/nAEHrW9EF

Making basic bytecode conversion available again to every learning developer

You can enable the DLL to use a pipe as well as some other settings at the top of dllmain.cpp. You are responsible for sending data to the pipe.

How To Build
Set configuration to Release x86 in Visual Studio and build

Note
This has no custom functions. It's a very small exploit and functions with only 2 source files. If you want to make custom functions (without abusing mid hooks or using temporarily uninlined functions), you'll need to:

Create a closure using closure offsets
Get the global table using a lua state offset
Create the string which should be the name of the function using string offsets
Write to the global table using table offsets, setting the key at the string you created to the closure you created
Implementing this in this repo would double or triple the amount of code, would be harder to maintain, and would be very confusing for beginners.



