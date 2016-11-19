# Dynamic-Array-Kernel 

## Usage

    BYTE_ARRAY arr;
    InitByteArray( &arr );

    AppendElementsByteArray( &arr, (PVOID)someBuffer, (ULONG)someBufferLength );

    FreeByteArray( &arr );
