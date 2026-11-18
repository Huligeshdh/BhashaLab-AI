
# Technology Decisions

## Decision 001: Librosa over Torchaudio

**Problem:**
We need an audio processing foundation for inspecting,
analyzing and visualizing speech recordings.

**Alternatives:**
- Librosa
- Torchaudio

**Decision:**
Use Librosa for the initial audio analysis pipeline.

**Reason:**
Librosa provides convenient tools for audio loading,
resampling, spectrograms and feature extraction.

**Trade-off:**
Torchaudio offers closer integration with PyTorch
and may be more appropriate for future model-training
pipelines.

**Validation:**
Compare audio loading, metadata extraction and
spectrogram generation on representative WAV files.

**Status:** Proposed — validate during implementation.
