# ANSI-Color-Codes-in-C
 This file defines constants and functions for adding ANSI color codes to C terminal output. It provides a simple way to colorize text printed to the console without needing to manually insert escape sequences.

<h3>Key aspects:</h3>

Constants define all common ANSI color codes for text styling.

Functions allow setting colors in a standardized way for print statements.

Portable across POSIX systems - utilizes widely supported ANSI escape codes.

Rather than a full-fledged API, this file encapsulates common color codes and offers a basic interface for coloring console text from C programs. Inclusion provides an easy means to dynamically set styles without low-level escape code handling.

Ideal for basic terminal output highlighting. The provided constants and functions standardize color use without deep library dependencies.


<h3>Usage</h3>
Here is an example usage of the ansicolor library:

```c
#include "ansicolor.h"

int main() {
   // Print text in different colors
   red();
   printf("This is red text\n");
   
   black();
   printf("This is black text\n");
   
   green();
   printf("This is green text\n");
   
   // Reset to default color
   default_color();
   
   // Print bold text
   printf(BOLD_RED "This is bold red text\n");
   
   // Underline cyan text
   printf(UNDERLINE_CYAN "This is underlined cyan text\n");
   
   // High intensity purple background
   printf(HIGH_INTENSTY_BACKGROUND_PURPLE "High intensity purple background\n");
   
   // Bold high intensity blue text
   printf(BOLD_HIGH_INTENSITY_TEXT_BLUE "Bold high intensity blue text\n");
   
   return 0;
}
```

To use:

Include ansicolor.h
Call provided color functions
Print colored text
Reset color as needed
