################################## BASIC DESCRIPTION ####################################

1) xudo is a modified sudo command that logs the commands run which can be later on debugged
[NOTES] : if xudo code is already installed please remove xudo code manually and install again


2) view your command logs using one of the commands as follows
                            1. nano ~/commandhistory.txt
                            2. nvim ~/commandhistory.txt
                            3. cat ~/commandhistory.txt


##################################### INSTALLATION #######################################


==================================  BASH INSTALLATION  ===================================

--------------------------- meathod 1 - copy and paste in ~/.bashrc


COPY HERE

################################################################################################
############################################  xudo  ############################################
################################################################################################

function xudo(){
  echo ''  >> ~/commandhistory.txt &&
  echo "command date_time_zone :" $(date "+%d-%B-%Y_%H-%M-%S_%Z=%:z") >> ~/commandhistory.txt &&
  echo $@ >> ~/commandhistory.txt &&
  sudo $@
}

################################################################################################
############################################  xudo  ############################################
################################################################################################

                                                                                  ENDD COPY HERE

step 1 :
         cd

step 2 :
         nano ~/.bashrc

step 3 :
         paste xudo code

step 4 :
         press ctrl+o

step 5 :
         press ctrl+x

step 6 :
         restart terminal








---------------------------  meathod 2 - copy and paste below command in terminal

step 1
      sudo cat xudo.bash >> ~/.bashrc

NOTES :  if xudo code is already installed remove existing xudo code and use this meathod

       step 1 : go to home dir
                cd

       step 2 : edit nano .bashrc
                nano ~/.bashrc

       step 3 : remove old xudo code
                find xudo code and delete

       step 4 : save edited file
                ctrl+o

       step 5 : exit from nano
                ctrl+x

       step 6 : install new xudo code 
                sudo cat xudo.bash >> ~/.bashrc

       step 7 : restart terminal 
                restart terminal







=====================================  2. FISH INSTALLATION  ===================================



COPY HERE

################################################################################################
############################################  xudo  ############################################
################################################################################################

function xudo
  echo ''  >> ~/commandhistory.txt &&
  echo "command date_time_zone :" (date "+%Y-%B-%d_%H-%M-%S_%Z %:z") >> ~/commandhistory.txt &&
  echo $argv >> ~/commandhistory.txt &&
  sudo $argv
end

################################################################################################
############################################  xudo  ############################################
################################################################################################



                                                                                   END COPY HERE

--------------------------- meathod 1 - copy and paste in ~/.config/fish/config.fish

step 1 : go to config.fish
         cd ~/.config/fish/

step 2 : edit config.fish
         nano ~/.config/fish/config.fish

step 3 : getting xudo code in fish
         paste xudo code

step 4 : save edited file
         press ctrl+o

step 5 : exit from nano
         press ctrl+x

step 6 : restart fish
         fish



--------------------------- meathod 2 - copy and paste below command in terminal


step 1 :
                  sudo cat xudo.fish >> ~/.config/fish/config.fish




NOTES : if old xudo code is installed remove old sudo code and install

step 1 : go to config.fish
         cd ~/.config/fish/

step 2 : edit config.fish
         nano ~/.config/fish/config.fish

step 3 : removing xudo code in config.fish
         paste xudo code

step 4 : save edited file
         press ctrl+o

step 5 : exit from nano
         press ctrl+x

step 6 : exit from nano
         sudo cat xudo.fish >> ~/.config/fish/config.fish

step 7 : restart fish
         fish

