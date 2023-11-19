# time-to-frequency
from scipy.signal import spectrogram
nfft = 500
overlap = 2
fs = 500
freqs , times, Sxx = spectrogram(a, fs=fs, nperseg=nfft, noverlap= overlap)
plt.pcolormesh(times, freqs, 10*np.log10(Sxx))
