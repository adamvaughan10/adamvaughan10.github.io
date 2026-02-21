---
layout: default
title: AI chatbot with MCP integration - meshIQ
---

<section class="section-card">
  <h2>AI Chatbot with MCP Integration - meshIQ</h2>
  <p class="tagline">MCP-powered Slack chatbot for meshIQ.</p>
</section>

<section class="section-card">
  <h3>Project Snapshot</h3>
  <ul>
    <li><strong>Project:</strong> AI chatbot with Model Context Protocol (MCP) integration</li>
    <li><strong>Company:</strong> meshIQ</li>
    <li><strong>Role:</strong> Software Engineer (solo build with senior engineer check-ins)</li>
    <li><strong>Timeline:</strong> ~1.5 months</li>
    <li><strong>Status:</strong> Proof of concept, ready for expansion</li>
    <li><strong>Stack:</strong> Python, Slack SDK, Anthropic MCP SDK + spec</li>
  </ul>
</section>

<section class="section-card">
  <h3>Overview</h3>
  <p>I rebuilt an existing proof of concept from the ground up to meet the Model Context Protocol (MCP) specification. The result is a Slack-based chatbot that allows meshIQ users to ask natural-language questions about middleware and receive grounded, auditable responses backed by meshIQ data.</p>
</section>

<section class="section-card">
  <h3>What I Built</h3>
  <ul>
    <li><strong>Slack chatbot:</strong> A production-style bot that connects to meshIQ data through MCP.</li>
    <li><strong>Memory for follow-ups:</strong> Conversation context keeps multi-turn questions seamless.</li>
    <li><strong>Two-stage reasoning:</strong> A fast route for simple queries, plus a planning loop for API-backed answers.</li>
    <li><strong>User auditability:</strong> Clear display of the LLM thought process and API call outcomes.</li>
  </ul>
</section>

<section class="section-card">
  <h3>How It Works</h3>
  <p>The chatbot uses a two-level reasoning model to balance speed, cost, and accuracy.</p>
  <ul>
    <li><strong>Level 1: Instant reasoning.</strong> Handles questions the LLM can answer from prior context or capability knowledge.</li>
    <li><strong>Level 2: Planning loop.</strong> Builds a task plan, selects meshIQ APIs, executes calls, validates results, and returns a structured summary including call status.</li>
  </ul>
  <p>This separation reduces token usage and improves response time while keeping answers grounded in actual platform data.</p>
  <figure class="project-figure project-figure-narrow">
    <img src="{{ '/assets/projects/meshIQ/first-level-reasoning.png' | relative_url }}" alt="First-level reasoning example showing instant response path">
    <figcaption class="tagline">Level 1 reasoning: fast answers from prior context without extra API calls.</figcaption>
  </figure>
</section>

<section class="section-card">
  <h3>Why It Matters</h3>
  <ul>
    <li><strong>Natural language access:</strong> Users can query middleware data without learning platform-specific tooling.</li>
    <li><strong>Operational clarity:</strong> API call outcomes are surfaced to build trust and enable auditing.</li>
    <li><strong>Extensible foundation:</strong> MCP makes it straightforward to add more meshIQ data sources and agentic workflows.</li>
  </ul>
</section>

<section class="section-card">
  <h3>Challenges &amp; Decisions</h3>
  <ul>
    <li><strong>Spec-compliant rebuild:</strong> I started from scratch to align with the MCP spec and remove PoC shortcuts.</li>
    <li><strong>Speed vs. accuracy:</strong> Two-stage reasoning kept responses fast without sacrificing data-backed answers.</li>
    <li><strong>Context handling:</strong> Memory design ensured follow-ups stayed consistent and relevant.</li>
  </ul>
</section>

<section class="section-card">
  <h3>Example Interactions</h3>
  <p>The three images below show the full loop: an initial request that triggers the planning loop and fails an API call, a follow-up reprompt with additional parameters that retries the same API and succeeds, and a final follow-up question answered from the already gathered data without re-entering the planning loop.</p>
  <figure class="project-figure project-figure-narrow">
    <img src="{{ '/assets/projects/meshIQ/thinking-loop.png' | relative_url }}" alt="Initial request showing the planning loop and a failed API call">
    <figcaption class="tagline">Initial request: planning loop runs, but the API call fails and is reported clearly.</figcaption>
  </figure>
  <figure class="project-figure project-figure-narrow">
    <img src="{{ '/assets/projects/meshIQ/FOLLOW-UP.png' | relative_url }}" alt="Follow-up request that re-runs the API call with new parameters">
    <figcaption class="tagline">Follow-up reprompt: extra parameters provided, the same API call reruns and succeeds.</figcaption>
  </figure>
  <figure class="project-figure project-figure-narrow">
    <img src="{{ '/assets/projects/meshIQ/follow-up2.png' | relative_url }}" alt="Second follow-up question answered from previously gathered data">
    <figcaption class="tagline">Second follow-up: question answered from prior results without another planning loop.</figcaption>
  </figure>
</section>

<section class="section-card">
  <h3>Future Potential</h3>
  <ul>
    <li>Integrate additional meshIQ datasets and operational views.</li>
    <li>Extend MCP interfaces to external agentic workflows.</li>
    <li>Productize the proof of concept into an internal knowledge assistant.</li>
  </ul>
</section>

<section class="section-card">
  <h3>Key Skills Demonstrated</h3>
  <ul>
    <li>LLM systems integration with Model Context Protocol (MCP)</li>
    <li>Python backend development</li>
    <li>Slack bot architecture</li>
    <li>Tooling for LLM reasoning, planning, and auditing</li>
    <li>Rapid onboarding to complex domain knowledge</li>
  </ul>
</section>
