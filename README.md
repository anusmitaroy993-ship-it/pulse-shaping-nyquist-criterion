# Pulse Shaping and the Nyquist Criterion

## Experiment 7

### Objectives

- Compare rectangular, sinc, raised-cosine and root-raised-cosine pulses.
- Study bandwidth and timing trade-offs through roll-off factor.
- Verify the Nyquist zero-crossing criterion.
- Study the cascade of transmitter and receiver RRC filters.

### Implementation

The experiment creates an upsampled symbol impulse train and applies different pulse-shaping filters.

Raised-cosine filters are tested for roll-off factors:

- α = 0
- α = 0.25
- α = 0.5
- α = 1

The experiment includes time-domain and frequency-domain analysis of the pulse responses.

A mandatory Nyquist zero-crossing validation is performed by sampling the overall raised-cosine response at integer symbol intervals.

The transmitter and receiver RRC filters are also cascaded to verify the overall raised-cosine response.

### Required Visualizations

- Pulse responses
- Frequency responses
- Pulse-shaped symbol stream
- Bandwidth versus roll-off factor
- Cascaded RRC response

### Mandatory Validation

The overall raised-cosine response is sampled at integer symbol intervals and the values are tabulated to verify the Nyquist zero-crossing criterion.

### Observations

Increasing the roll-off factor increases the required bandwidth.

The raised-cosine pulse maintains zero crossings at integer symbol intervals, satisfying the Nyquist criterion.

The cascaded transmitter and receiver RRC filters produce an overall raised-cosine response.

### Files Included

- `pulse_shaping_nyquist.py` - Python source code
- `Experiment_7_Pulse_Shaping_Nyquist_Criterion.ipynb` - Google Colab notebook
- `Experiment_7_Pulse_Shaping_Nyquist_Criterion.pdf` - Experiment report
