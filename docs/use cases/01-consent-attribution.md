# Use Case 1: Consent & Attribution

## Trigger
User wants to know if consent was given or is required, and what attribution obligations exist.

---

## Q1: What's your situation?

- [ ] My work may have been used without permission
- [ ] I want to use someone else's work
- [ ] I'm building a tool/product that uses others' work
- [ ] Something else → [text input] → **logged**

---

## Path A: My work may have been used

### Q2a: What type of work?

- [ ] Sound recording (released track, stems, samples)
- [ ] Voice / vocal performance
- [ ] Composition / melody / lyrics
- [ ] Something else → [text input] → **logged**

### Q3a: What do you know?

- [ ] I found my work in a known dataset
- [ ] I suspect it was used but have no proof
- [ ] An AI output sounds like my work
- [ ] Not sure where to start
- [ ] None of these fit → [text input] → **logged**

### Outputs (A):

**If found in dataset:**
- Document evidence (screenshots, dataset name, URL)
- Check if you gave consent (platform ToS, distribution agreements)
- File GDPR data subject access request (EU) to demand removal
- Consider legal consultation if commercial harm

**If suspected but no proof:**
- Search: Have I Been Trained, Spawning.ai, dataset documentation
- Check if distributor (DistroKid, TuneCore, etc.) licensed your work to AI companies
- Document timeline of your releases vs. model training dates

**If AI output sounds like your work:**
- This is harder to prove—similarity ≠ training inclusion
- Document the output, compare to your original
- Consider: is this copyright infringement (output) or training data issue (input)?

**If not sure where to start:**
- Start with Have I Been Trained (https://haveibeentrained.com)
- Check your distributor's AI policy
- Review any contracts for AI/ML clauses

**Sources:**
- GDPR Article 15 (right of access), Article 17 (right to erasure)
- EU AI Act transparency requirements (Article 53)
- Spawning.ai, Have I Been Trained

---

## Path B: I want to use someone else's work

### Q2b: What do you want to use?

- [ ] Voice / likeness of a real person
- [ ] Sound recording / sample
- [ ] Composition / melody
- [ ] Something else → [text input] → **logged**

### Q3b (Voice/likeness): What's the context?

- [ ] Real person, identifiable voice
- [ ] Synthetic voice trained on real person
- [ ] Fully synthetic, no real person reference
- [ ] Not sure → **logged**

### Outputs (B - Voice/likeness):

**Real person, identifiable:**
- Explicit consent required (written, specific to use case)
- Attribution likely required (check agreement)
- Right of publicity laws vary by jurisdiction (US state-level, EU personality rights)
- High risk if used commercially without consent

**Synthetic trained on real person:**
- Same obligations as real voice—consent from original person
- "Deepfake" regulations emerging (EU AI Act Article 52: disclosure required)
- Platform ToS may prohibit (check distribution/streaming policies)

**Fully synthetic, no real person:**
- Lower risk, but check:
  - AI tool's ToS (do they claim ownership?)
  - Platform policies (Spotify, YouTube, etc. disclosure rules)
- Attribution to AI tool may be required by their license

**Sources:**
- EU AI Act Article 52 (transparency for synthetic media)
- GDPR Article 9 (biometric data as special category)
- US: State right of publicity laws (CA, TN, NY)

---

### Q3b (Sound recording): What's the context?

- [ ] Sample from released track
- [ ] Stem/multitrack from released track
- [ ] Sound from sample library
- [ ] AI-generated sound trained on existing recordings
- [ ] Not sure → **logged**

### Outputs (B - Sound recording):

**Sample from released track:**
- Clearance required (master + publishing rights)
- Contact label (master) and publisher (composition)
- No "fair use" assumption for music sampling in most jurisdictions

**Stem/multitrack:**
- Same as sample—clearance required
- Stems don't have separate/lesser rights

**Sample library:**
- Check license type (royalty-free, rights-managed, AI-training exclusion?)
- Many libraries now have AI-specific clauses—read ToS
- Attribution may be required depending on license

**AI-generated sound trained on others' work:**
- You inherit the ethical/legal ambiguity of the training data
- Check AI tool's documentation on training data provenance
- If tool trained on unlicensed data, your output may be legally risky
- Consider "ethical AI" alternatives with documented consent

**Sources:**
- Copyright law (jurisdiction-specific)
- Sample library ToS
- AI tool documentation / model cards

---

## Path C: I'm building a tool/product

### Q2c: What's your role?

- [ ] Training a model on audio/music data
- [ ] Using a pre-trained model in my product
- [ ] Building a platform where users upload/generate content
- [ ] Something else → [text input] → **logged**

### Q3c (Training a model): Data source?

- [ ] Licensed dataset (documented consent)
- [ ] Scraped from public internet
- [ ] User-uploaded content
- [ ] Mix of sources
- [ ] Not sure → **logged**

### Outputs (C - Training):

**Licensed dataset:**
- Document the license, keep records
- Verify license covers AI/ML training (many older licenses don't)
- Be prepared to prove provenance if challenged

**Scraped from public internet:**
- High legal risk in EU (GDPR, EU AI Act)
- "Public" ≠ "free to use for training"
- Opt-out mechanisms required (EU AI Act Article 53)
- Check robots.txt, ToS of source sites

**User-uploaded content:**
- Your ToS must explicitly cover AI training use
- Users must be informed and consent
- Consider opt-in vs opt-out (opt-in is safer)
- GDPR: data subject rights apply

**Mix of sources:**
- Document each source separately
- Weakest link determines overall risk
- Consider data auditing tools

**Sources:**
- EU AI Act Articles 52, 53
- GDPR Articles 6, 7 (lawful basis, consent)
- US Copyright Office guidance on AI training

---

## Edge Case Logging

Any "Something else" or "None of these fit" response captures:
- Timestamp
- Path taken (e.g., Q1 → A → Q2a → Q3a)
- User text input
- Optional: contact for follow-up (user choice)

Logged edge cases reviewed monthly for v1.1 use case expansion.
