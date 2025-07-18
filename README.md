# 🧠 DecentraTutor - WCHL 2025 Submission

> A decentralized AI tutor for math and science built on Internet Computer (ICP).

## 🚀 Overview

**DecentraTutor** is an on chain learning assistant that answers math/science questions using AI and stores student learning history on ICP. Built for the AI - Decentralized Intelligence track of WCHL 2025.

## ✨ Features

- AI-powered explanations to math/science questions
- On-chain question logging using ICP Rust Canisters
- Minimal, clean React frontend
- Community feedback (upvotes/downvotes on answers)

## 📸 Demo Screenshots

> _(Add screenshots here before submission)_

## 📽️ Demo Video

> [Link to your demo video (YouTube, Loom, etc.)]

## 🔧 Tech Stack

| Layer       | Stack                          |
|-------------|--------------------------------|
| Frontend    | React + TailwindCSS            |
| Backend     | ICP Canisters (Rust)           |
| AI Model    | OpenAI API or local LLM (off-chain initially) |
| Deployment  | dfx + Internet Computer        |

## 🧱 Architecture

- User asks a question on the frontend
- React triggers an API call to a Rust based canister
- Canister logs the query and returns the AI generated response
- Future enhancement: deploy small LLM models fully on chain

## 🛠️ Setup Instructions

```bash
git clone https://github.com/YOUR_USERNAME/decentratutor.git
cd decentratutor

# Backend
cd backend
dfx start background
dfx deploy

# Frontend
cd ../frontend
npm install
npm run dev
