Relational Database Training Projects

This repository contains 3 small Rails applications built to practice relational database modeling and seeding. The focus is on models, migrations, and seeds — no controllers or views.

1. FreeDoc – Book Your Doctor

A Doctolib-style app to manage doctors, patients, and appointments.

Models: Doctor, Patient, Appointment.

Relations:

One doctor ↔ many appointments.

One patient ↔ many appointments.

Doctors and patients linked through appointments (N-N).

Extras:

City model (doctors, patients, and appointments belong to a city).

Specialty model (many-to-many with doctors).

2. Dog Airbnb – Dog Walking Platform

A matching service between dogs and dogsitters.

Models: Dog, Dogsitter, Stroll.

Relations:

Many dogs ↔ many dogsitters through strolls.

Extras:

City model (each dog and dogsitter belongs to one city).

3. The Gossip Project – Social Gossip App

A social network to share gossips and comments.

Models: User, City, Gossip, Tag, PrivateMessage, Comment, Like.

Relations:

User ↔ many gossips, comments, likes, private messages.

Gossip ↔ many tags (N-N), many comments, many likes.

Private messages with sender and multiple recipients.

Extras:

Nested comments (polymorphism).

Usage

Clone the repo(s).

Run migrations:

rails db:migrate


Seed the database with sample data:

rails db:seed


These apps are designed for pair programming practice at [THP].