# 🔄 Self-Critique Workflow

A reusable workflow for stress-testing research ideas before presenting them to advisors, reviewers, or search committees. Developed from real experience: by pre-rehearsing critiques, external feedback becomes validation rather than attack.

---

## Step 1: Generate the Idea (AI-Assisted)

**Prompt:**
```
I have a research idea about [X]. Help me flesh it out into a 1-page description including:
- Motivation: Why does this problem matter?
- Approach: What will I do?
- Expected Contribution: What's new?
- Novelty: How is this different from existing work?
```

## Step 2: Generate the Harshest Review (AI as Reviewer)

**Prompt:**
```
You are a senior HCI/NLP/SE reviewer known for being extremely tough and specific. Write a detailed review of this research idea with:
- 3 major weaknesses
- 2 minor weaknesses

Be specific, harsh, and realistic. Consider:
- Novelty: Has this been done before? What's truly new?
- Technical depth: Is the approach rigorous enough?
- Evaluation plan: How would you actually validate this?
- Scope: Is this too broad or too narrow?
- Positioning: How does this compare to [specific related work]?

Do NOT be nice. I need to hear the worst.
```

### Optional: Add domain-specific reviewers

**For NLP venues:**
```
Now review this as an ACL/EMNLP reviewer. Focus on: dataset quality, baseline comparisons, reproducibility, and whether the NLP contribution is substantial or just an application.
```

**For SE venues:**
```
Now review this as an ICSE/FSE reviewer. Focus on: practical relevance, scalability, developer study design, and whether the SE community would find this impactful.
```

**For HCI venues:**
```
Now review this as a CHI reviewer. Focus on: user study rigor, design rationale, theoretical grounding, and whether the contribution goes beyond "we built a system."
```

## Step 3: Write Your Own Rebuttal

⚠️ **Do this yourself. Do NOT let AI write it.**

For each weakness:
- ✅ Can defend → Write your response
- ❌ Can't defend → This is a real weakness. Flag it.

The ones you can't rebut are the ones that need fixing.

## Step 4: Revise the Idea

**Prompt:**
```
Based on my rebuttal below, help me revise the original idea to address the weaknesses I couldn't fully defend:

[Paste your rebuttal]

Focus on strengthening the weak points while preserving the core contribution.
```

## Step 5: Search Committee Simulation (Optional, for Job Market Prep)

**Prompt:**
```
You are a search committee member at a top CS department. I just gave a 45-minute job talk based on this work. 

What would you ask during Q&A? What concerns would you raise in the closed-door committee discussion afterward? Consider:
- Does this person have a clear research identity?
- Is there a viable 5-year research agenda here?
- Would this person get tenure?
- How does this compare to other candidates on the market?
```

## Step 6: Advisor Meeting Simulation (Optional)

**Prompt:**
```
You are a senior professor who gives high-level feedback but rarely does hands-on work. Critique this idea the way you would in a 1-on-1 meeting: focus on framing, positioning, and whether the story is compelling. Point out what's unclear or unconvincing.
```

---

## 🎯 When to Use This Workflow

- Before presenting a new idea to your advisor
- Before submitting a paper (run Step 2 with venue-specific reviewer)
- Before a job talk (run Step 5)
- Before any high-stakes conversation about your research
- Whenever you feel anxious about someone criticizing your work

## 💡 Why This Works

The pain of criticism comes from being unprepared, not from the criticism itself. When you've already rehearsed the worst-case scenario, real feedback feels like confirmation rather than attack. You shift from reactive to proactive.
