# get_next_line
Get next line function alone with only the libft parts it uses.
Done with no research into existing programs. This program reads from the filedescriptor given and returns one full line
Not compatiable with other reading functions since it would read past what it needs and store that for later (side effect of read() )

Very fast, very scalable and very memory efficient. I used linked lists for the fds given so theres no hard coded cap on those.
The linked lists only uses memory as needed and even deletes the list node when you hit the end of file.

Some optimisations are possible but its more than efficient enough and other projects call.
