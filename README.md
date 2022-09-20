# Fuzzing Essentials: Training for Federal Employees and Contractors

## Course Description

The world is facing a software security crisis.

Github reports there are 570 times more developers  than cybersecurity experts.
Worse, 87% of organizations say they can't keep up with automating security
testing, so we’re fielding code faster than we can secure it.

The result. The status quo technologies have left  offense with a permanent
advantage.

In 2014, DARPA asked what if there was an autopilot for application security?
What if we could teach machines to find vulnerabilities at machine speeds,
rather than human speeds. They called this the Cyber Grand Challenge, and put up
a $2 million dollar cash prize for anyone who could complete it.  We unleashed
Mayhem, and showed that autonomous appsec is possible.

We didn’t stop there. At ForAllSecure, we believe it’s fundamentally necessary
to make application security more autonomous.  There simply aren’t enough human
security experts to beat all attackers.

We’ve taken the theory, ideas, and tools from the Cyber Grand Challenge and
built the product Mayhem you can use today.  Mayhem uses techniques DARPA
called revolutionary, and we call AI fuzzing.

AI Fuzzing is intelligent fuzzing. Fuzzing is a term used to describe algorithms
that automatically sample the program input space to elicit new program
behaviors.  Fuzzing has evolved since “trash can” fuzzing from punch-cards and
random behavior to “AI Fuzzing”, which uses advanced program analysis
techniques.  For example, Mayhem (and indeed all top competitors) used
techniques like portfolio analysis, symbolic execution, and
instrumentation-guided heuristics as part of their fuzzing tool set in the
Cyber Grand Challenge.

In this course, we will introduce you to the techniques that underpin fuzzing,
and show you how to incorporate those techniques into your organization. These
techniques will allow you to:

1. Find and prove vulnerabilities with zero false
positives.  Developers love the actual proof-of-concept that demonstrates the
problem, just like a human hacker would provide. Managers love that every
report is actionable. And program managers love the savings from avoiding false
positives, which can account for 25%+ of your security budget.

2. Automatically and continuously improve the test suite, which eliminates
unknowns caused by un-tested or under-tested code. Organizations report up to
70% of their developer time is building test scenarios. Behavior-based fuzzing
expands code coverage for the price of a CPU hour rather than a human work hour.

You will learn with hands-on examples using Mayhem. However, the course is also
generally applicable to anyone who wants to learn how to fuzz, including using
open source tools like AFL, libfuzzer, and honggfuzz.

We’re excited to have you join us.  We hope you take away fundamental new
skills. But moreso, we also hope you come away with a passion for making appsec
more autonomous.

## Agenda

- Introductions
- Course Overview
- Lab 1: Fuzzing Lighttpd
    - 1a. Fuzz with the Mayhem UI.
        - Outcomes:
            - Log in to the Mayhem UI
            - Launch lighttpd fuzzing campaign
            - Find vulnerability.
    - 1b. Fuzzing Lighttpd (CLI)
        - Outcomes:
            - Log in to the Mayhem CLI
            - Launch lighttpd fuzzing campaign
            - Find vulnerability.
- Lab 2: Reproducing Vulnerabilities Locally
    - Outcomes:
        - Download test cases.
        - Run lighttpd in a container “locally”.
        - “Replay” vulnerability.
- Four Corners of Application Security
    - Outcomes:
        - Understanding 4 corners of appsec
        - Identify why binary analysis (vs source) is critical
        - Describe coverage, and how it relates to a program behavior
            - Function coverage
            - Node Coverage
            - Edge Coverage
            - Path Coverage
    - Revisiting Lab 1:
        - Interpret fuzzing coverage output
        - Understand how security testing relates to software reliability testing and standards.
- Tutorial Testme example
    - Mayhem package
    - Docker
- Challenge: Fuzz $n$-day
    - Docker Image: dbrumley/libbw64:latest
    - Program: /libbw64/libbw64/build/examples/bw64_read_write
    - Solution: Ask!
- Symbolic Execution Primer
    - Outcomes:
        - Understand what Mayhem does under the hood.
- Zero-days:
    - Toyota, Bosch, and Honda open-source, oh my!
- Networking:
    - Tutorial bacsrv
    - Example: exploiting netflix dial https://github.com/ForAllSecure/VulnerabilitiesLab/blob/master/netflix-cve-2019-10028/mayhem/dial/Mayhemfile
- OSS Fuzzers
    - AFL
    - libfuzzer
        - Advanced Challenge: Fuzz ConnMan, Exploit Car!
- Fuzzing Harnesses
    - libxml lab

## Schedule

* Day 1: 1100 - 1830 ET
  * Lunch: 1200 - 1300 ET
  * 5 minute break every ~1 hour.
  * 15 minute break every ~2 hours.
  * Social 1800-1830

* Day 2: 1100 - 1600 ET
  * Lunch: 1200 - 1300 ET
  * 5 minute break every ~1 hour.
  * 15 minute break every ~2 hours.

## Links

* [Mayhem Instance (https://training.forallsecure.com)](https://training.forallsecure.com)
* [Lab 1](lab1.md)
* [Lab 2](lab2.md)
* [Mayhem Community](https://community.forallsecure.com)

## Resources

* [Linux CLI Reference](assets/Linux_Useful_Commands.pdf)
* [slido (for Survey Questions)](https://www.sli.do/)
* [Adversarial Testing Training and Certification Course](assets/Adversarial_Testing_Training_and_Certification_Offering.pdf)
