all: README.md

README.md: guessinggame.sh
    echo "Unix Workbench course project" > README.md
    echo "\n**Description^^: Make a program called guessinggame.sh. It will ask to guess for the number of files in the directory, tell if its hig or low and congrats if correct." >> README.md
    echo -n "\n^^Make date^^: " >> README.md
    date >> README.md
    echo -n "\n^^Number of lines in guessinggame.sh:**" >> README.md
    grep -c '' guessinggame.sh >> README.md

clean:
    rm README.md
