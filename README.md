# Unified_Code_Count
Unified Code Count is a Software Metrics Tool that parses over 20 different programming languages to find 
Logical and Physical source lines of code, counts keywords and various operators, math function names, etc. 
and cyclomatic complexity for a given language and then generates various reports.  

This release includes significant performance enhancements and capability for multiple Threads.
Approximate speed up you will see is between 2x and 3x faster.

This is a change from UCC 2013_04 as released by University of Southern California.
Original 2013_04 source files can be found at http://csse.usc.edu/ucc
Written in cross platform C++

This variation includes the contents the of original 2013_04 release 
with some modified and added source files and some documents briefly describing changes.

### Easy build with CMake
- Download CMake for windows from https://cmake.org/
- Execute the build.bat or the following commands inside src path:
```bash
cmake -G "Visual Studio 14 2015"
cmake --build . --config Release
```
- And build will be ends successfully

(Below is contents of Read_Me.txt from the zip file)
====================================================

Read_Me.txt    for Unified Code Count 2013_04 with Threading and other improvements
June 6, 2015

Files found here

Counting Rules                           documents - 1 doc per language parser group
                                            23 files
src                                      sources needed to build UCC Thread version
                                            90 files with 30 different language parsers

license.txt                              original from UCC
Makefile                                 original from UCC
Read_Me.txt                              the file you are reading now...
UCC.2008.vcproj                          original from UCC
UCC.2010.vcxproj                         original from UCC
UCC.2010.vcxproj.filters                 original from UCC
UCC.2012.vcxproj                         original from UCC
UCC.2012.vcxproj.filters                 original from UCC
UCC_CA_Profile_DIFF_No_DUP_0.png         screen shot of AMD CodeAnalyst profiler in use
UCC_CA_Profile_DIFF_No_DUP_Details.txt   profiling/improving Differencing procedures
UCC_CA_Profile_DUP_No_DIFF_Details.txt   profiling/improving Duplication checking procedures
UCC_Multithreading_Notes.doc             text and screen shots giving some background during development
UCC_Release_Notes_Threads_2013_04.txt    descriptions of changes and some tips (strongly suggested reading)
UCC_release_notes_v.2013.04.pdf          original Release notes
UCC_user_manual_v.2013.04.pdf            original User manual

For all else:
You can Register and get the original UCC 2013_04 distribution including docs at
http://csse.usc.edu/ucc_wp/

		License:
I adhere to terms as stated in the license.txt file in this directory from USC.
I have no other terms.
The software changes are freely available and with the same limitations.
I have no other license file for anyone to mull over.

		Acknowledgements:

To: Center for Systems and Software Engineering
         University of Southern California
                       and
      All those elsewhere who have contributed.
    Thanks to all the people past and present that built UCC.
    I am happy to give back to a tool I have used to find complexity nuggets.

To: Boost C++ libraries creators, contributors and maintainers.
    I am humbled by the insights gained from using Boost.
    Thanks so much.

To: Jeff Preshing for contributing a cross platform Semaphore library.
    The semaphore library sema.h was an excellent fit 
    after a slight edit to not require C++ 2011 features.
    Enjoyed reading your web site and the analogies and illustrations.
    Thank you.

To: AMD CodeAnalyst team and whatever you are working on now.
    Thanks for building such an excellent profiler that made my work much easier.

To: KDiff3 team for building such an effective visual difference utility.
    This tool literally saved me hours of time that I would have needed
    checking all the various UCC output options trying to use other methods.
    Thanks for a best in class visual differencer.

As for me,
I tried to leave some sensible comments along with the working code...
Hopefully these changes will be merged into the original UCC baseline future versions.

Enjoy!
Randy Maxwell
