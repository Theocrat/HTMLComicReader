# HTMLComicReader

The aim of this project is to implement a simple HTML comic reader. It should ideally consist of a single HTML page, and it should use client-side Javascript and CSS to implement a simple applet for reading comic books one page at a time. First, this README will define key terms required to state the objectives of this project.

### Comic book

A comic book is defined as a collection of images which satisfy the following properties:
  1. They are all in the same image format.
  2. They are all located in the same directory.
  3. Their filenames, apart from the extension, are numbers from 1 to some integer number *n*, where *n* is the number of such images, with no number skipped or repeated.
  4. Additionally, the images must be in a format that a browser can open.

As can be observed, the "comic book" need not even be a comic book proper. It can be any numbered collection of images in a single format and within a single directory. As of now, the project is at an initial stage and hence not very ambitious. As of now, the applet requires all file names to be simple positive integers, with rounding zeros suppressed (for instance, `01.jpg` does not count). Also, this applet does not allow multiple subdirectories within the main comic book directory at this stage.

Additionally, we are working under the assumption that the comic book is in the hard disk or some such storage device.

### Other Definitions

**Page:** Each image within the comic book directory is called a page.

**File Path:** The _absolute file path_ of the directory which contains the images.

### TODO:

  1. Implement aesthetics, potentially by including small arrowhead icons for page transitions.
  2. Implement a feature whereby filenames with explicit zeroes to the left of the page number can be handled. For instance, the popular comic Gunnerkrigg Court has six explicit digits per page name. The first page is named `000001.jpg`, for instance.
  3. Some comics are divided into chapters, which are subdirectories within the main comic directory. The project does not handle this kind of multichapter comic as of now, but this will have to be implemented.
  4. Comics which are available on the web in distant servers should also be viewable in a future version of this project.
  5. A more interactive selection for the File Path would make the applet more user-friendly.
  6. It would be nice if a simple installer could be implemented, which would allow easy installation of the reader.
