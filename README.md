trailing-spaces-removal
=======================
Simple trailing spaces removal script.


Instructions:
-------------

Installation:

        $ git clone git@github.com:lenguyenthedat/trailing-spaces-removal.git
        $ ./install # cp tsrm /usr/local/bin/

Running on local directory:

        $ ./tsrm .
        Input folder: .
        Going remove trailing white spaces for:
        ./README.md
        ./tsrm
        ./test/some_file_with_trailing_spaces.txt
        ./test/test_child_folder/another_file_with_trailing_spaces.txt
        Are you sure to proceed? y

Files changed:

        $ git status
        On branch master
        Changes not staged for commit:
          (use "git add <file>..." to update what will be committed)
          (use "git checkout -- <file>..." to discard changes in working directory)

            modified:   test/some_file_with_trailing_spaces.txt
            modified:   test/test_child_folder/another_file_with_trailing_spaces.txt

        no changes added to commit (use "git add" and/or "git commit -a")

Files diff:

        $ git diff
        diff --git a/test/some_file_with_trailing_spaces.txt b/test/some_file_with_trailing_spaces.txt
        index 7a41e98..41c2ad9 100644
        --- a/test/some_file_with_trailing_spaces.txt
        +++ b/test/some_file_with_trailing_spaces.txt
        @@ -1,3 +1,3 @@
        -
        -Try removing me
        +
        +Try removing me

        diff --git a/test/test_child_folder/another_file_with_trailing_spaces.txt b/test/test_child_folder/another_file_with_trailing_spaces.txt
        index ef8ec92..01d793f 100644
        --- a/test/test_child_folder/another_file_with_trailing_spaces.txt
        +++ b/test/test_child_folder/another_file_with_trailing_spaces.txt
        @@ -1,4 +1,3 @@
        -
        - trailing spaces
        - ftw
        -
        \ No newline at end of file
        +
        + trailing spaces
        + ftw
