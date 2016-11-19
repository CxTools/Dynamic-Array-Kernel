# Dynamic-Array-Kernel 

Dynamic array for windows kernel development. I recently had to develop something similar to STL vector, but compatible in kernel mode, since I had chunks of unknown sizes coming in that I had to parse. So, I created this. I couldn't find anything like this anywhere online, though I didn't look too hard. But it works, and it works well. 

## Usage

    BYTE_ARRAY arr;
    InitByteArray( &arr );

    AppendElementsByteArray( &arr, (PVOID)someBuffer, (ULONG)someBufferLength );

    FreeByteArray( &arr );
