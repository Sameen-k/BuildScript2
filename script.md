#!/bin/bash 

echo "1 - ssh" 
echo "2 - scp"
read -p "select an option to continue" choice

#For SSH
if [[ $choice == "1" ]]
then 
    read -p "please enter remote system ip address: " ip
    read -p "please enter the username: " username
        ssh "$username@$ip"
#for scp 
elif [[ $choice == "2" ]]
then 
    read -p "please enter remote system ip address:" remip
    read -p "please enter the username:" user2
    echo "1 - local to remote"
    echo "2 - remote to local"
    read -p "please choose an option" choice2
    read -p "please enter source file location:" source
    read -p "please enter destination file location:" destination
        if [[ $choice2 == 1 ]]
        then 
            scp "$source" "$user2@remip" : "$destination"
        elif [[ "$choice2 == 2 ]] 
        then
            scp "$source" "$user2@remip" : "$destination"
#the above elif literally doesnt work im so confused :(
else 
    echo "that's not an option! please try again!"
