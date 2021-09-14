#!/usr/bin/python
# -*- coding: utf-8 -*-


class SoftwareEngineer:
    def __init__(self):
        self.name = "Mokhinur Abdurakhimova"
        self.position = "Computer Vision Engineer"
        self.location = "Tashkent, Uzbekistan"
        self.skills = [
            "Software Engineering",
            "Data Science",

        ]
        self.skills.insert(0, "Computer Vision and Deep Learning")

    def greeting(self):
        print(
            """Hello folks!

This is {name}, I live in {location}. I am a student at National University and recently I am focusing on {focus} for my personal growth.

I have many interests, but most of them are {skills}. I like solving complex logic tasks and enjoy while coding""".format(
                name=self.name,
                location=self.location,
                focus=self.skills[0],
                skills=", ".join(self.skills[1:]),
            )
        )


me = SoftwareEngineer()
me.greeting()
