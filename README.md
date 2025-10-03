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

Usage

Clone the repo(s).

Run migrations:

rails db:migrate


Seed the database with sample data:

rails db:seed


These apps are designed for pair programming practice at [THP].
