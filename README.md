# Dynamic-Array-Kernel 

Dynamic array for windows kernel development. I recently had to develop something similar to STL vector, but compatible in kernel mode, since I had chunks of unknown sizes coming in that I had to parse. So, I created this. I couldn't find anything like this anywhere online, though I didn't look too hard. But it works, and it works well. 

## Usage

    BYTE_ARRAY arr;
    InitByteArray( &arr );

    AppendElementsByteArray( &arr, (PVOID)someBuffer, (ULONG)someBufferLength );

    FreeByteArray( &arr );
   
## License
    
Copyright (C) 2016 dude719

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with this program. If not, see http://www.gnu.org/licenses/.
