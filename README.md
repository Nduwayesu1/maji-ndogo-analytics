# maji-ndogo-analytics

# Maji Ndogo Digital Twin: From Notepad to a Farm That Can Reason

## The Business Problem

Maji Ndogo's Ministry of Agriculture ran its farms on paper. Field details lived on a notepad, tractors moved only when someone pushed a button, and nobody could ask the system how much of a field was planted, which machines were low on fuel, or what each farm had harvested. Without reliable records and basic logic, the ministry couldn't plan, save fuel or trust its own numbers. [CONFIRM: one sentence on what was at stake]

## The Tech Stack

Core Python only, with no libraries and no databases. I used data structures (lists, tuples, sets, dictionaries), control flow, comprehensions and function design. I did this on purpose: a Digital Twin built from the language's own building blocks shows I understand how the tools underneath every data library work.

## The Deliverable

**Step 1: Clean, trustworthy records.** [CONFIRM: what module 1 built]

![Clean field records](images/01-clean-records.png)

**Step 2: The system decides when a tractor needs fuel.** The same fuel reading produces 'Low', 'OK' or 'Full' depending on the fraction of the tank left, so a machine can be flagged before it runs dry.

![Fuel status check](images/02-fuel-status.png)

**Step 3: The tractor stops the moment it meets the pipe.** It plants every cell up to the obstacle and never plants past it, so a physical hazard is handled in code instead of by a person watching.

![Tractor stops at obstacle](images/03-obstacle-stop.png)

**Step 4: One line finds every vehicle with a small tank.** A single comprehension returns the low-fuel models for any fleet size, keeping the original order.

![Low-fuel fleet check](images/04-low-fuel-models.png)

**Step 5: Two farms' crop plans are compared cleanly.** The system reports what both farms grow, what only one grows and the full catalogue, with duplicates removed.

![Crop plan comparison](images/05-crop-plans.png)

**Step 6: Harvests accumulate instead of overwriting.** A second reading for the same farm and crop adds to the total (2050 kg becomes 2550 kg), so the registry stays accurate through the season.

![Harvest registry](images/06-harvest-registry.png)

## The "So What?"

The ministry went from a notepad to a model of its farms that can count what is planted, flag low fuel, stop at obstacles and keep a running harvest record. [CONFIRM: your own one or two sentences on what Sanaa's team can now do that they couldn't before]
