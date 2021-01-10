# Référence API

> [**WINDOWS API REFERENCE**](https://docs.microsoft.com/en-us/windows/console/console-reference)

## GetStdHandle

Récupère un gestionnaire vers le périphérique standard spécifié (entrée standard, sortie standard ou erreur standard).

```c
HANDLE WINAPI GetStdHandle(_In_ DWORD nStdHandle);
```

### Paramètre :

|VALEUR|TAILLE|CODE|
|:--:|:--:|:--:|
|**STD_INPUT_HANDLE**|DWORD|-10|
|**STD_OUTPUT_HANDLE**|DWORD|-11|
|**STD_ERROR_HANDLE**|DWORD|-12|

## WriteConsole

```c
BOOL WINAPI WriteConsole(_In_ HANDLE hConsoleOutput, _In_ const VOID *lpBuffer, _In_ DWORD nNumberOfCharsToWrite, _Out_opt_ LPDWORD lpNumberOfCharsWritten, _Reserved_ LPVOID lpReserved);
```