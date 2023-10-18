για το bandit0 ο κωδικός δίνεται, οπότε συνδέομαι με ssh στο bandit0 
και στο readme στο οποίο μπαίνω με την εντολή cat βρίσκω τον κωδικό για το bandit1.
στη συνέχεια, μπαίνω στο φάκελο - με την εντολή cat./- και βρίσκω τον κωδικό για το bandit2.
κάθε φόρα που βρίσκω επόμενο κωδικό κάνω exit και συνδέομαι με αυτόν στο επόμενο αριθμητικά bandit.
για το 3, χρησιμοποιώ την εντολή cat spaces\ in\ this\ filename.
για το 4, μπαίνω στο inhere με cd inhere και με την εντολή ls -al βλέπω τα κρυφά αρχεία και με την cat .hidden μπαίνω στο συγκεκριμένο.
για το 5, μπαίνω στο inhere με cd inhere, ls για να δω τα περιεχόμενα και με find . -type f | xargs file (για να βρω το human readable, το file07) και cat ./-file07.
για το 6, cd inhere, find . -type f -size 1033c(για τα bytes) ! -executable και μετα cat ./maybehere07/.file2
για το 7, find / -type f -user bandit7 -group bandit6 -size 33c και απο τα αποτελέσματα αντιγράφω τη διεύθυνση του αρχείου με τον κωδικό και κανω cat cat /var/lib/dpkg/info/bandit7.password
για το 8, cat data.txt για να δω το περιεχόμενο του data και μετά strings data.txt | grep "millionth" για να εμφανίσει συγκεκριμένα μετα τη λέξη millionth.
για το 9, cat data.txt για τα περιεχόμενα και sort data.txt για να βάλει τα παροόμοια μαζί και sort data.txt | uniq -c 
για το 10, strings data.txt | grep "=" που εμφανίζει τα strings που ξεκινάνε με =
για το 11, cat data.txt και base64 -d data.txt για αποκωδικοποίηση του base64 τύπου.
