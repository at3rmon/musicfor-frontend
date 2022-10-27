<script setup>
import { RouterLink } from "vue-router";
import { library } from "@fortawesome/fontawesome-svg-core";
import { FontAwesomeIcon } from "@fortawesome/vue-fontawesome";
import {
  faDesktop,
  faCalendarDays,
  faGraduationCap,
  faTrainSubway,
  faWifi,
  faEarthEurope,
  faFilm,
  faHeartPulse,
  faWheelchair,
} from "@fortawesome/free-solid-svg-icons";
library.add(
  faDesktop,
  faCalendarDays,
  faGraduationCap,
  faTrainSubway,
  faWifi,
  faEarthEurope,
  faFilm,
  faHeartPulse,
  faWheelchair
);
</script>
<template>
  <div class="home container max-w-6xl mx-auto">
    <section class="space-y-6">
      <h1 class="font-bold text-center text-5xl">Welcome to MusicFor</h1>
      <p class="text-center text-lg">
        Το MUSICFOR είναι μία Σύγχρονη Μουσική Σχολή!
      </p>
      <p class="text-center text-lg">
        Το MUSICFOR ακολουθεί ένα εκπαιδευτικό πρόγραμμα που καλύπτει τις
        ανάγκες των σπουδαστών του, δίνοντας τη δυνατότητα απόκτησης
        <strong>Διεθνώς Αναγνωρισμένων Πτυχίων</strong> και
        <strong>Διπλωμάτων</strong> σε διάφορους τομείς της μουσικής εκπαίδευσης
        σε συνεργασία με το <strong>No 1 Πανεπιστήμιο του Λονδίνου</strong> για
        τις μοντέρνες σπουδές, το University of West London!
      </p>
      <p class="text-center text-lg">
        Φιλοξενεί ένα σύνολο μουσικών, δασκάλων και μαθημάτων που καλύπτουν
        μεγάλο εύρος της μουσικής εκπαίδευσης, ενώ ταυτόχρονα αποτελεί μία πύλη
        επικοινωνίας με αναγνωρισμένους μουσικούς της
        <strong>παγκόσμιας</strong> σύγχρονης μουσικής σκηνής, όπως οι John
        Scofield, John Abercrombie, Julian Lage, Lage Lund, Bill Frisell, Kurt
        Rosenwinkel, Jonathan Kreisberg, Larry Goldings, Bill Stewart, Paul
        Gilbert, Aaron Parks, Peter Bernstein, Allan Mednard, Larry Carlton,
        Adam Levy, Greg Howe, Colin Stranahan, Andy McKee, Guthrie Govan, Doug
        Aldrich και άλλοι.
      </p>
    </section>

    <div class="divider"></div>

    <section class="grid grid-cols-3 gap-6">
      <div class="card w-full bg-base-100 shadow-2xl hover:bg-base-300">
        <div class="card-body items-center text-center">
          <font-awesome-icon icon="fa-solid fa-desktop" class="text-6xl" />
          <h2 class="card-title">Technologically Advanced</h2>
          <p>
            Οι εγκαταστάσεις μας παρέχουν σύγχρονο εξοπλισμό, τόσο στις
            αίθουσες, όσο και στο στούντιό μας.
          </p>
          <div class="card-actions">
            <RouterLink to="#" class="btn btn-primary">Read More</RouterLink>
          </div>
        </div>
      </div>
      <div class="card w-full bg-base-100 shadow-2xl hover:bg-base-300">
        <div class="card-body items-center text-center">
          <font-awesome-icon
            icon="fa-solid fa-calendar-days"
            class="text-6xl"
          />
          <h2 class="card-title">Planning Events</h2>
          <p>
            Διοργανώνουμε συνεχώς σεμινάρια και συναυλίες με μεγάλα ονόματα της
            παγκόσμιας μουσικής σκηνής.
          </p>
          <div class="card-actions">
            <RouterLink to="#" class="btn btn-primary">Read More</RouterLink>
          </div>
        </div>
      </div>
      <div class="card w-full bg-base-100 shadow-2xl hover:bg-base-300">
        <div class="card-body items-center text-center">
          <font-awesome-icon
            icon="fa-solid fa-graduation-cap"
            class="text-6xl"
          />
          <h2 class="card-title">Accredited by UWL</h2>
          <p>
            Οι σπουδαστές μας μπορούν να παρακολουθήσουν μαθήματα προσαρμοσμένα
            στις εξετάσεις του LCM/RGT.
          </p>
          <div class="card-actions">
            <RouterLink to="#" class="btn btn-primary">Read More</RouterLink>
          </div>
        </div>
      </div>
      <div class="card w-full bg-base-100 shadow-2xl hover:bg-base-300">
        <div class="card-body items-center text-center">
          <font-awesome-icon icon="fa-solid fa-train-subway" class="text-6xl" />
          <h2 class="card-title">Easy Access</h2>
          <p>
            Πολύ εύκολη πρόσβαση μέσω Μετρό (ή και λεωφορείων), καθώς
            βρισκόμαστε λίγα μέτρα απ' το σταθμό Κεραμεικός.
          </p>
        </div>
      </div>
      <div class="card w-full bg-base-100 shadow-2xl hover:bg-base-300">
        <div class="card-body items-center text-center">
          <font-awesome-icon icon="fa-solid fa-wifi" class="text-6xl" />
          <h2 class="card-title">Free Wi-Fi</h2>
          <p>
            Δωρεάν διαθέσιμο WiFi σε όλους τους χώρους του musicfor, για τους
            σπουδαστές μας, αλλά και τους επισκέπτες.
          </p>
        </div>
      </div>
      <div class="card w-full bg-base-100 shadow-2xl hover:bg-base-300">
        <div class="card-body items-center text-center">
          <font-awesome-icon icon="fa-solid fa-earth-europe" class="text-6xl" />
          <h2 class="card-title">International collaborations</h2>
          <p>
            Το musicfor και πολλοί καθηγητές του έχουν λάβει μέρος σε διεθνείς
            συνεργασίες, είτε στην Ελλάδα είτε στο εξωτερικό.
          </p>
        </div>
      </div>
      <div class="card w-full bg-base-100 shadow-2xl hover:bg-base-300">
        <div class="card-body items-center text-center">
          <font-awesome-icon icon="fa-solid fa-film" class="text-6xl" />
          <h2 class="card-title">Live streaming</h2>
          <p>
            Οι καθηγητές μας θα παρουσιάζουν ένα δωρεάν μάθημα, το οποίο θα
            κινηματογραφείται σε live streaming.
          </p>
        </div>
      </div>
      <div class="card w-full bg-base-100 shadow-2xl hover:bg-base-300">
        <div class="card-body items-center text-center">
          <font-awesome-icon icon="fa-solid fa-heart-pulse" class="text-6xl" />
          <h2 class="card-title">Heart of Events</h2>
          <p>
            Μέσα στην καρδιά των καλλιτεχνικών εξελίξεων, κοντά στο Τεχνόπολις
            και σε συνεργασία με το gazARTE.
          </p>
        </div>
      </div>
      <div class="card w-full bg-base-100 shadow-2xl hover:bg-base-300">
        <div class="card-body items-center text-center">
          <font-awesome-icon icon="fa-solid fa-wheelchair" class="text-6xl" />
          <h2 class="card-title">Ramp Access</h2>
          <p>
            Εύκολη πρόσβαση για τα άτομα με ειδικές ικανότητες ή κινητικά
            προβλήματα, μέσω ράμπας.
          </p>
        </div>
      </div>
    </section>
  </div>
</template>
