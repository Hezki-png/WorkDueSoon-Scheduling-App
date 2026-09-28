# WorkDueSoon-Scheduling-App
Offline college assignment and test tracker. Items are an array of objects saved as JSON on the phone. Each view filters the array, sorts by due time (O(n log n)), then groups by day in one pass. Late items float to the top in red; done ones go to History. Countdowns are due minus now, redone every 30s. Backups merge with a hash map by id.
