# Install
sudo apt-get install git

# Initialize the git in ubuntu
git config --global user.name "Michelle2hungry"
git config --global user.email "1264908491@qq.com"
'''
    To see the git configuration:
        git config --list
'''

# Create a new repository in Github.com
(operate online)
e.g. gittest

# Make directory in local server
mkdir gittest

# Creat a file
cd gittest
~/gittest/: vim git-ubuntu.md
(write content into file)

# Initialize
git init

# Add and Commit
git add git-ubuntu.md
git commit -m "first commit"
git remote add origin http://github.com/Michelle2hungry/gittest.git
'''
    if remote origin have already exists and you want to reset it:
        git remote rm origin
'''

# Push to master
git push -u origin master
'''
    if fail to connect:
        env | grep -i proxy
        unset *_proxy
'''

# Need help in git
git <verb> --help
git help <verb>

# Two scenarios using git
## 1) Tracking local repository
    '''some files don't be track
    touch .gitignore
    git status
