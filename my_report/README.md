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

Eπειδή αντιμετώπισα πολλά προβλήματα με την αναγνώριση των μαρκερ, ξανάρχισα τον κώδικα από την αρχή με αυτό που έχετε στο δικό σας repository με το Hiro. Μάλιστα, αφού δοκιμάστηκε, το Hiro δουλεύει καλά. Έφτιαξα το μάρκερ με το dpsd μου στη ζωγραφική, και μάλιστα γέμισα το background με ανοιχτό γκρι με rgb 240,240,240 όπως διάβασα σε αυτή τη <a href="https://github.com/jeromeetienne/AR.js/issues/164#issuecomment-328830663">συζήτηση</a>. Αφού το έκανα αυτό και ένα crop την εικόνα, την ανέβασα στο  <a href="https://jeromeetienne.github.io/AR.js/three.js/examples/marker-training/examples/generator.html">AR.js Training</a> ώστε να φτιάξω το pattern. Επίσης πρόσεξα το ratio να είναι 0.50 όπως αυτό του Hiro σε περίπτωση που όπως με το γκρι χρώμα ήταν ένας λόγος που δε μου αναγνώριζε το pattern. Με τον ίδιο τρόπο έφτιαξα και τα άλλα markers με το υδρογόνο και το οξυγόνο που βρήκα σαν αρχικά png στα assets. Αφού τα έκανα, κατέβασα την εικόνα του pattern και του αρχείου patt και από τα 3, και τα ανέβασα όλα στο assets. Μετά πήγα στον κώδικα και τον έφτιαξα για να διαβάζει τα pattern. Έκανα αντιγραφή 2 σειρές κώδικα pattern από  <a href="https://aframe.io/blog/arjs/">εδώ</a> στο σημείο που είχε τα pattern kanji & Hiro και απλά έβαλα το preset δίπλα στο type και το άλλαξα σε custom. Επίσης, άλλαξα τα URL και έβαλα αυτά από το assets τα .patt. Στη αρχή είχα βάλει όλο το URL όπως φαίνεται στην εικόνα που έστειλα στα issues και μετά από τη δική σας βοήθεια και λίγο ψάξιμο εκεί άλλαξα το path σε '/assets/pattern-dpsd19014.patt'. Παρόλα αυτά τα pattern δε λειτουργούσαν ακόμα. Έκανα λογαριασμό στο glitch.com γιατί είδα ένα <a href="https://www.youtube.com/watch?v=xXJ5KDMlcJQ">βίντεο</a> όπου κάποιος έκανε σχεδόν το ίδιο assignment 
 και γενικά από κει και σε άλλους κώδικες από το github που έψαχναν <a href="https://github.com/jeromeetienne/AR.js/issues/164#issuecomment-332065686">αρκετοί</a> είχαν διπλά brackets [ " ] και όχι [ ' ] αλλά αφού δοκίμασα και τα 2 τίποτα δε δούλευε. Προσπάθησα να δω τι θα γινόταν αν έσβηνα το preset ή το type και δεν υπ'ηρχε καμία διαφορά. Δοκίμασα και πολλές φορές από το κινητό μου καθώς η κάμερα είναι πολύ καλύερη και πάλι τίποτα. Προχώρισα λοιπόν στο να βάλω την εικόνα και το text κάτω από το marker dpsd19014. Από τα issues βρήκα τις σειρές κώδικα που ήθελα καθώς και από ψάξιμο στο github από άλλους χρήστες κατέληξα σε αυτό που έγραψα. Κατέβασα την εικόνα και την ανέβασα στα assets και έβαλα το path/URL στον κώδικα. Ονόμασα την εικόνα μου στο id όπου την όρισα σαν a-asset και την κάλεσα στο a-image. Ακόμα με βάσει κάποια σχόλια άλλαξα το a-marker σε a-marker-camera αλλά δεν είχε καμιά διαφορά. Έκανα δοκιμή με το έτοιμο dpsd που ήταν ήδη στα assets και δεν δούλευε ούτε αυτό. Έκανα δοκιμή σε local server που υποθέτω ήταν από ότι διάβασα στο διαδίκτυο να πατήσω το index από τα αρχεία μου που είχα κατεβάσει όλο το AR zip και δε δούλεψε ξανά. Για επεξήγηση, τα μαρκερ τα ελεγχα αν δουλεύουν με εμφάνιση ενός box. επίσης τον κώδικα τον άφησα όπου το 1 URL το πήρα από την επιλογή copy URL απο το asset οπου ειχε μέσα και το κομμάτι του marker_based ενώ τα άλα τα έγραψα όπως μου υποδείξατε εσείς και οι άλλοι από τα λινκ που είναι παραπάνω. Επίσης σχετικά με αυτό δεν ξέρω αν έχει σημασία στο URL να υπάρχει το [ / ] πριν το assets. Με βάση άλλα σχόλια, το έβγαλα γιατί το άτομο που το έλεγε είχε αρκετό θετικό δείκτη όπου υποστήριζε ότι έτσι θα δούλευε. 
 
ΔΙΟΡΘΩΣΗ 19-5-22
Μετά από λίγο ψάξιμο κατάλαβα λίγα λάθη στον κώδικα και όταν τα διόρθωσα τα μάρκερ δούλεψαν. Προσπάθησα να φτιάξω καλά το positioning για την εικόνα και τα γράμματα που θα εμφανίζονται στο μαρκερ dpsd. Προχώρησα στο επόμενο βήμα που ήταν με τα τρισδιάστατα μοντέλα. Τον κώδικα στο script το πήρα από τα issues του μαθήματος και Έβαλα και τους 2 μάρκερ οξ + υδρογ με το ίδιο 3d object το οποίο είναι το Oxygen_molecule, το οποίο το πήρα από εδώ. Έγραψα την επανάληψη για τα 3dmodel, τις 2 για το Oxygen_molecule και το 3d για το Water_drop (το οποίο το πήρα από τη βιβλιοθήκη 3d onjects του υπολογιστή), όπου αν η απόσταση μεταξύ των μάρκερ είναι μικρότερη από 2, το water-drop θα φαίνεται ενώ τα Oxygen_molecule όχι και το αντίστροφο αν η απόσταση είναι μεγαλύτερη από 2. Το μοντέλο για το oxygen-hydrogen το βρήκα <a href="https://sketchfab.com/3d-models/oxygen-molecule-c536fd0a0b754fc4856ee7eb85ee0b63">εδώ</a> όπου το κατέβασα σε μορφή gltf. Το μοντέλο του νερού το έκανα convert από gltf σε glb <a href="https://anyconv.com/gltf-converter/">εδώ</a>




# 3rd Deliverable 

Αρχικά πήρα τον κώδικα από το syros.index για το 3d αντικειμενο του magnemite, εβαλα το δικό μου 3δ από τα assets του location_based. Μπήκα στο google maps και πήρα συντεταγμένες του σημείου ενδιαφερόντος. Έβαλα τις συντεταγμένες στο latitude - longtitude και τις άλλαξα λίγο για το simulation για να φανεί στη κάμερα. Το αντικείμενο το πήρα από <a href="https://www.turbosquid.com/3d-models/republic-china-flag-max-free/663944">εδώ</a>. Για το syros.index χρησιμοποίησα την ίδια λογική. Μέσα στο entity έβαλα ένα τεξτ που το πήρα από τη βικιπαίδεια <a href="https://el.wikipedia.org/wiki/%CE%94%CE%AE%CE%BC%CE%BF%CF%82_%CE%A3%CF%8D%CF%81%CE%BF%CF%85_
  _%CE%95%CF%81%CE%BC%CE%BF%CF%8D%CF%80%CE%BF%CE%BB%CE%B7%CF%82"> εδώ</a>. Γα τη κάμερα βρήκα αυτόν τον κώδικα για το rig <a href="https://aframe.io/docs/1.3.0/components/camera.html"> Aframe</a>. Έπειτα ήθελα να κάνω τον μηχανισμό όπου πατώντας το 3d αντικείμενο να εμφανιζόταν ένα τεξτ. Έβαλα το τεξτ μέσα στο entity. Άλλαξα το αρχείο από glb σε gltf. Είδα ότο έχει διαφορά, καθώς όταν ανανεώνω τη σελίδα τουθ index βλεπω μια μαυρίλα σε ορισμένα σημεία, κάτι που πιστεύω έχει να κάνει με το gps και ότι βρίσκομαι μέσα στο αντικείμενο. Πήρα το clickable από depository άλλων χρηστών που είδα. Ύστερα αφού μπήκα από τον προσωπικό μου υπολογιστή, τίποτα δε δούλευε, παρότι δεν άλλαξα τον κλωδικα. Άλλαξα συντεταγμένες, position, έσβησα τα rotation, στο Alt+ctrl+i δεν εμφανίζωνταν ούτε κείμενο ούτε το 3d. Άλλαξα τον κώδικα για το κείμενο με βάση <a href="https://aframe.io/docs/1.3.0/components/text.html">εδώ</a>. Όποτε προσπαθώ να το τρέξω μου εμφανίζει εκέινη τη μπλε εικόνα που φορτώνει.


# Conclusions


# Sources
<p><a href="https://www.npmjs.com/package/aframe-particle-system-component">particle system component</a></p>
<p><a href="https://www.npmjs.com/package/aframe-speech-command-component">speech command</a></p>
<p><a href="https://www.youtube.com/watch?v=xXJ5KDMlcJQ">το βίντεο από το glitch</a></p>
<p><a href="https://aframe.io/blog/arjs/">κώδικα για custom patterns</a></p>
<p><a href="https://github.com/jeromeetienne/AR.js/issues/164#issuecomment-328830663">issue για πατερν που δε δουλεύει</a></p>
<p><a href="https://jeromeetienne.github.io/AR.js/three.js/examples/marker-training/examples/generator.html">φτιάξιμο μάρκερ</a></p>
<p><a href="https://github.com/jeromeetienne/AR.js/issues/164#issuecomment-332065686">issue για πατερν που δε δουλεύει για μπρακετς</a></p>
<p><a href="https://sketchfab.com/3d-models/oxygen-molecule-c536fd0a0b754fc4856ee7eb85ee0b63">3d oxygen and hydrogen molecule</a>.<p>
<p><a href="https://anyconv.com/gltf-converter/">gltf converter</a><p>
<p><a href="https://el.wikipedia.org/wiki/%CE%94%CE%AE%CE%BC%CE%BF%CF%82_%CE%A3%CF%8D%CF%81%CE%BF%CF%85_
  _%CE%95%CF%81%CE%BC%CE%BF%CF%8D%CF%80%CE%BF%CE%BB%CE%B7%CF%82">τεξτ βικιπαιδεια</a><p>
<p><a href="https://www.turbosquid.com/3d-models/republic-china-flag-max-free/663944">3d model china for location based</a></p>
<p><a href="https://aframe.io/docs/1.3.0/components/camera.html">camera rig</a></p>
<p><a href="https://aframe.io/docs/1.3.0/components/text.html"> link for text</a></p>
  
