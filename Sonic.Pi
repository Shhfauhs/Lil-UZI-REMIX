# Lil-UZI-REMIX


#I JUST WANNA ROCK-LIL UZI VERT
define :main_notes do
  play :eb4
  sleep 2
  play :f4
  sleep 2
  play :gb4
  sleep 2
  play :db5
  sleep 2
  play :db5
  sleep 2
  play :r
  sleep 0.5
  play :bb4
  sleep 0.5
  play :eb5
  sleep 1
  play :db5
  sleep 2
  play :f5
  sleep 1
  play :bb5
  sleep 1
end

liar = "C:/Users/Luis Rios/Documents/Audacity/BBBB.wav"

use_bpm 150
use_synth :dsaw
notes = [:eb4, :f4, :gb4, :db5, :db5, :r, :bb4, :eb5, :db5, :f5, :bb5]
s = [2, 2, 2, 2, 2, 0.5, 0.5, 1, 2, 1, 1]
i = 0


sample liar
sleep 4
live_loop :uzi do
  use_synth_defaults sustain: 2
  11.times do
    play notes [i]
    sleep s [i]
    i = i + 1
  end
  i = 0
end


sleep 15
live_loop :doo do
  4.times do
    sample :drum_bass_hard
    sleep 0.5
  end
  sleep 14
end

with_fx :bpf do
  use_synth_defaults sustain: 2
  1.times do
    main_notes
  end
end
