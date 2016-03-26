Unofficial Draft CS 3114 Style Guide for Web-Cat Submissions
============================================================

Introduction
------------

At this time, this is a work in progress style guide created for the purpose of reducing ambiguity in project grading for CS 3114 at Virginia Tech. Active discussions and pull requests are encouraged.

Project File Structure
----------------------

### Source File Structure

When structuring the source files of your project, use a flat directory structure; that is, your source files will all be contained in the project "src" directory. Any subdirectories in the project will be ignored.

***Rationale:*** Web-Cat currently has issues with processing submissions with source folder subdirectories/packages.

Formatting
----------

### Column Limit: 80 characters

All source code lines must not exceed 80 characters in length.

***Rationale:*** Setting a maximum line length facilitates higher readability for the code within editor buffers of varying column width.

### Source Code Length Limit Per File: 500 Lines

All source code files must adhere to a maximum length of 500 lines.

***Rationale:*** Limiting the length of a file increases readability by limiting the amount of content a reader must keep track of within that file. This well help the TAs and instructors provide assistance and grade the submissions.

Programming Practices
---------------------

### Identifier Scope

Entities should reside in as small of a scope as necessary. That is: nested classes, members, and methods that are implementation details of a single class should be declared private. A single java source should expose as few identifiers as necessary.

***Rationale:*** As it is, Web-Cat's limitations require that student-written code declares classes within the default package. This presents the possibility of name space collisions: two entities with the same identifier being defined within the default package. It is a good practice to expose as few entities as possible to the "outside world" to prevent collisions.
