# Gitatlas 🌌

> Visual repository intelligence — understand how code evolves, not just what changed

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/)
[![React 18](https://img.shields.io/badge/react-18-61dafb.svg)](https://reactjs.org/)

---

## What is Gitatlas?

Gitatlas is a visual interface for exploring GitHub repositories through their history.

Instead of scrolling through commits line by line, you navigate a repository as a continuous timeline — a sequence of checkpoints that represent how the system evolved over time.

Each commit becomes a visible unit of progress. Relationships between commits become paths. The repository becomes something you can explore, not just read.

---

## The Idea

GitHub shows commits as a list.
Gitatlas treats them as a structure.

A repository is modeled as a directed timeline where:

* commits are checkpoints
* changes are transitions
* contributors are participants in the evolution
* time is represented spatially

The result is a view where development feels sequential, contextual, and navigable.

---

## Features

* **Visual Timeline**
  Commit history rendered as a flowing graph instead of a linear log

* **Checkpoint-Based Exploration**
  Each commit is an interactive node positioned along a directional path

* **Commit Inspection**
  Expand any checkpoint to view its metadata, changes, and context

* **Repository Insights**
  Activity patterns, contribution frequency, and change volume

* **Contributor Visibility**
  Understand who contributed and when

* **Risk Detection ⚠️**
  Highlights commits containing sensitive patterns such as exposed keys or configuration files

* **Context Summaries 🧠**
  Concise explanations of what a commit represents

---

## How it works

You provide a repository URL.
Gitatlas processes its commit history and constructs a structured timeline.

From there:

* the timeline is rendered as a directed flow (top-left to bottom)
* nodes appear as checkpoints along this path
* edges represent progression
* interactions reveal deeper layers of information

The system prioritizes readability and continuity over raw detail.

---

## Interaction

The interface is built around two simple actions:

**Hover**
Quickly inspect a commit without leaving the timeline

* commit message
* author
* timestamp

**Click**
Open a detailed view of the selected commit

* summary of the change
* contributors involved
* files modified
* additions and deletions

This allows both scanning and deep inspection without breaking flow.

---

## What you can understand with Gitatlas

* when major features were introduced
* how frequently development occurred
* who contributed to specific parts of the system
* where significant changes happened
* when potential issues or risky changes were introduced

It turns repository history into something interpretable at a glance.

---

## Architecture

Gitatlas is structured into four layers:

* **Data Layer**
  Fetches commit data using GitHub APIs

* **Processing Layer**
  Normalizes relationships between commits and structures the timeline

* **Analysis Layer**
  Classifies commits, aggregates metrics, and detects anomalies

* **Visualization Layer**
  Renders the graph and handles interaction

---

## Use Cases

* onboarding into unfamiliar repositories
* understanding system evolution before making changes
* debugging by tracing when behavior changed
* reviewing contributions across time
* presenting project history in a visual format

---

## Limitations

* very large repositories may require optimization or partial rendering
* commit classification is heuristic-based
* visualization assumes relatively consistent commit structure

---

## Team

Built by: Abhinav and Neha


* [Abhinav Bombale]
* [Neha Lende]
