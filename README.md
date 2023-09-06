# BuildScript2

NOTES:

Before this neatly organized script I had echo commands followed by read commands which was a very inefficient and confusing way to format a script. I was luckily introduced to “read -p” by fellow cohort members and was able to turn my ugly script into a much more decent looking one like this. 

I attempted to try to use the case command but due to bad planning on my part I couldn’t figure out how to get it to work in time so I decided to just stick to the slightly familiar if/elif statements. Though I was lucky enough to see an example of functioning case statements which was very nice. 

ISSUES WITH THE SCRIPT:

I was honestly unable to figure out how to actually set up the ssh connection within the script. Without the ssh being established manually (copying ssh key-gen from local machine and pasting into authorized keys in our remote machine) how can we set it up automatically. I couldn’t not seem to figure out how to set up 

My script can’t actually copy files so  its broken, I’m sure it has something to do with the if/then statements but I can’t figure out whats wrong. It could be the format or the scp command itself and I can’t figure out how to differentiate between remote - local and local - remote in my command

Resources:
https://www.youtube.com/watch?v=G852MWw48BY&ab_channel=linuxhint
https://www.youtube.com/watch?v=QALD8r0JQPY&ab_channel=ShawnPowers
