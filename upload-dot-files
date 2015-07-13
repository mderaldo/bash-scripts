#!/bin/sh

echo "=====> Uploading dotFiles"

#Clone dotFiles repository
git clone git@github.com:mderaldo/dotfiles.git $HOME/dotfiles
pwd

echo "=====> Copying files"
#Updating dotFiles
cp $HOME/.gitconfig $HOME/dotfiles/
cp $HOME/.zlogin $HOME/dotfiles/
cp $HOME/.zlogout $HOME/dotfiles/
cp $HOME/.zpreztorc $HOME/dotfiles/
cp $HOME/.zprofile $HOME/dotfiles/
cp $HOME/.zshenv $HOME/dotfiles/
cp $HOME/.zshrc $HOME/dotfiles/


#Clone dotFiles repository
cd $HOME/dotfiles

pwd
#Add new files
git add .

#Git commit new version
git commit -m "Updating the dotfiles."

echo "=====> Pushing diff"
#Up
git push origin master 

#Clone dotFiles repository
git clone git@github.com:mderaldo/dotfiles.git

#Remove dotfiles repository
cd $HOME/
rm -rf $HOME/dotfiles

echo "=====> Done!"