# Lesson: Interaction Design

### First and Last Name: Ζωή Γαλάνη
### University Registration Number: dpsd19014
### GitHub Personal Profile: ZoiGalanidpsd19014
### Augmented Reality Personal Repository: https://github.com/ZoiGalanidpsd19014/Augmented-Reality

# Introduction

# Summary


# 1st Deliverable

Πήγα στο κώδικα και έκανα αντιγραφή επικόλληση το κομμάτι με το κύβο. Άλλαξα το id και το geometry primitive σε κύλινδρο (cylinder) και σφαίρα (sphere) αντίστοιχα. Άλλαξα τις διαστάσεις, τα position και τα χρώματα. όλα αυτά βρίσκονται μέσα στις αγκύλες του a-marker preset = 'hiro' δηλαδή θα εμφανιστούν μόνο όταν το σύμβολο εμφανίζεται στη κάμερα. Από τη πηγή https://www.npmjs.com/package/aframe-particle-system-component πήρα τους κώδικες για το χιόνι, και πρόσθεσα και βροχή. στο particleCount ορισα αριθμο νιφαδων, στο size το μεγεθός τους, στο στο opacity την ορατοτητα και στο maxage τον χρονο που θα βρισκονται ορατα στο πλαίσιο.

Για την φωνητική εντολή πήγα στην πηγή https://www.npmjs.com/package/aframe-speech-command-component και αντέγραψα/επικόλλησα τις εντολές για το aframe-speech-command-component, annyang και speech-command.
  όπου άλλαξα το command και το id.


# 2nd Deliverable

Eπειδή αντιμετώπισα πολλά προβλήματα με την αναγνώριση των μαρκερ, ξανάρχισα τον κώδικα από την αρχή με αυτό που έχετε στο δικό σας repository με το Hiro. Μάλιστα, αφού δοκιμάστηκε, το Hiro δουλεύει καλά. Έφτιαξα το μάρκερ με το dpsd μου στη ζωγραφική, και μάλιστα γέμισα το background με ανοιχτό γκρι με rgb 240,240,240 όπως διάβασα σε αυτή τη συζήτηση. <a href="https://github.com/jeromeetienne/AR.js/issues/164#issuecomment-328830663"></a>. Αφού το έκανα αυτό και ένα crop την εικόνα, την ανέβασα στο AR.js Training <a href="https://jeromeetienne.github.io/AR.js/three.js/examples/marker-training/examples/generator.html"></a> ώστε να φτιάξω το pattern. Επίσης πρόσεξα το ratio να είναι 0.50 όπως αυτό του Hiro σε περίπτωση που όπως με το γκρι χρώμα ήταν ένας λόγος που δε μου αναγνώριζε το pattern. Με τον ίδιο τρόπο έφτιαξα και τα άλλα markers με το υδρογόνο και το οξυγόνο που βρήκα σαν αρχικά png στα assets. Αφού τα έκανα, κατέβασα την εικόνα του pattern και του αρχείου patt και από τα 3, και τα ανέβασα όλα στο assets. Μετά πήγα στον κώδικα και τον έφτιαξα για να διαβάζει τα pattern. Έκανα αντιγραφή 2 σειρές κώδικα pattern από εδώ <a href="https://aframe.io/blog/arjs/"></a> στο σημείο που είχε τα pattern kanji & Hiro και απλά έβαλα το preset δίπλα στο type και το άλλαξα σε custom. Επίσης, άλλαξα τα URL και έβαλα αυτά από το assets τα .patt. Στη αρχή είχα βάλει όλο το URL όπως φαίνεται στην εικόνα που έστειλα στα issues και μετά από τη δική σας βοήθεια και λίγο ψάξιμο εκεί άλλαξα το path σε '/assets/pattern-dpsd19014.patt'. Παρόλα αυτά τα pattern δε λειτουργούσαν ακόμα. Έκανα λογαριασμό στο glitch.com γιατί είδα ένα βίντεο όπου κάποιος έκανε σχεδόν το ίδιο assignment <a href="https://www.youtube.com/watch?v=xXJ5KDMlcJQ"></a>
 και γενικά από κει και σε άλλους κώδικες από το github που έψαχνα αρκετοί είχαν διπλά brackets [ " ] και όχι [ ' ] αλλά αφού δοκίμασα και τα 2 τίποτα δε δούλευε. Προσπάθησα να δω τι θα γινόταν αν έσβηνα το preset ή το type και δεν υπ'ηρχε καμία διαφορά. Δοκίμασα και πολλές φορές από το κινητό μου καθώς η κάμερα είναι πολύ καλύερη και πάλι τίποτα. Προχώρισα λοιπόν στο να βάλω την εικόνα και το text κάτω από το marker dpsd19014. Από τα issues βρήκα τις σειρές κώδικα που ήθελα καθώς και από ψάξιμο στο github από άλλους χρήστες κατέληξα σε αυτό που έγραψα. Κατέβασα την εικόνα και την ανέβασα στα assets και έβαλα το path/URL στον κώδικα. Ονόμασα την εικόνα μου στο id όπου την όρισα σαν a-asset και την κάλεσα στο a-image. Ακόμα με βάσει κάποια σχόλια άλλαξα το a-marker σε a-marker-camera αλλά δεν είχε καμιά διαφορά. Έκανα δοκιμή με το έτοιμο dpsd που ήταν ήδη στα assets και δεν δούλευε ούτε αυτό. Έκανα δοκιμή σε local server που υποθέτω ήταν από ότι διάβασα στο διαδίκτυο να πατήσω το index από τα αρχεία μου που είχα κατεβάσει όλο το AR zip και δε δούλεψε ξανά.


# 3rd Deliverable 


# Conclusions


# Sources
<a href="https://www.npmjs.com/package/aframe-particle-system-component"></a>
<a href="https://www.npmjs.com/package/aframe-speech-command-component"></a>
<a href="https://www.youtube.com/watch?v=xXJ5KDMlcJQ"></a>
<a href="https://aframe.io/blog/arjs/"></a>
<a href="https://github.com/jeromeetienne/AR.js/issues/164#issuecomment-328830663"></a>
<a href="https://jeromeetienne.github.io/AR.js/three.js/examples/marker-training/examples/generator.html"></a> 
