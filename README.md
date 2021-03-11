# nodejs-midi

INSTALL LIBASOUND
--------------


   3. Open a terminal window and do the following

      #make sure your system is fully up to date
      sudo apt-get update
      sudo apt-get upgrade
      sudo apt-get dist-upgrade

      #If the kernel was updated, reboot

   4. In the terminal window, again run:

      #forcefully remove the ALSA libraries
      sudo dpkg -r --force-depends libasound2 libasound2-data

      #install ALSA libraries including the DEV package
      sudo apt-get install libasound2 libasound2-data libasound2-dev


----------------
phil@phil-OptiPlex-790:~/nodejs-files$ npm install midi

> midi@1.0.0 install /home/phil/nodejs-files/node_modules/midi
> node-gyp rebuild

make : on entre dans le répertoire « /home/phil/nodejs-files/node_modules/midi/build »
  CXX(target) Release/obj.target/midi/src/lib/RtMidi/RtMidi.o
  CXX(target) Release/obj.target/midi/src/input.o
  CXX(target) Release/obj.target/midi/src/output.o
  CXX(target) Release/obj.target/midi/src/midi.o
  SOLINK_MODULE(target) Release/obj.target/midi.node
  COPY Release/midi.node
make : on quitte le répertoire « /home/phil/nodejs-files/node_modules/midi/build »
npm WARN saveError ENOENT: no such file or directory, open '/home/phil/nodejs-files/package.json'
npm notice created a lockfile as package-lock.json. You should commit this file.
npm WARN enoent ENOENT: no such file or directory, open '/home/phil/nodejs-files/package.json'
npm WARN nodejs-files No description
npm WARN nodejs-files No repository field.
npm WARN nodejs-files No README data
npm WARN nodejs-files No license field.

+ midi@1.0.0
added 4 packages from 14 contributors and audited 4 packages in 9.227s
found 0 vulnerabilities



   ╭───────────────────────────────────────────────────────────────╮
  │                                                               │
   │      New major version of npm available! 6.14.10 → 7.5.2      │
   │   Changelog: https://github.com/npm/cli/releases/tag/v7.5.2   │
   │               Run npm install -g npm to update!               │
   │                                                               │
   ╰───────────────────────────────────────────────────────────────╯

phil@phil-OptiPlex-790:~/nodejs-files$ 


-----------------
/usr/include/alsa/alisp.h
/usr/include/alsa/asoundef.h
/usr/include/alsa/asoundlib.h
/usr/include/alsa/conf.h
/usr/include/alsa/control.h
/usr/include/alsa/control_external.h
/usr/include/alsa/error.h
/usr/include/alsa/global.h
/usr/include/alsa/hwdep.h
/usr/include/alsa/input.h
/usr/include/alsa/mixer.h
/usr/include/alsa/mixer_abst.h
/usr/include/alsa/output.h
/usr/include/alsa/pcm.h
/usr/include/alsa/pcm_external.h
/usr/include/alsa/pcm_extplug.h
/usr/include/alsa/pcm_ioplug.h
/usr/include/alsa/pcm_old.h
/usr/include/alsa/pcm_plugin.h
/usr/include/alsa/pcm_rate.h
/usr/include/alsa/rawmidi.h
/usr/include/alsa/seq.h
/usr/include/alsa/seq_event.h
/usr/include/alsa/seq_midi_event.h
/usr/include/alsa/seqmid.h
/usr/include/alsa/timer.h
/usr/include/alsa/topology.h
/usr/include/alsa/use-case.h
/usr/include/alsa/version.h
/usr/include/alsa/sound/asoc.h
/usr/include/alsa/sound/asound_fm.h
/usr/include/alsa/sound/emu10k1.h
/usr/include/alsa/sound/hdsp.h
/usr/include/alsa/sound/hdspm.h
/usr/include/alsa/sound/sb16_csp.h
/usr/include/alsa/sound/sscape_ioctl.h
/usr/include/alsa/sound/tlv.h
/usr/include/alsa/sound/type_compat.h
/usr/include/sys/asoundlib.h
/usr/lib/x86_64-linux-gnu/libasound.so
/usr/lib/x86_64-linux-gnu/pkgconfig/alsa.pc
/usr/share/aclocal/alsa.m4
/usr/share/doc/libasound2-dev/changelog.Debian.gz
/usr/share/doc/libasound2-dev/copyright
/usr/share/doc/libasound2-dev/examples/audio_time.c.gz
/usr/share/doc/libasound2-dev/examples/chmap.c.gz
/usr/share/doc/libasound2-dev/examples/client_event_filter.c
/usr/share/doc/libasound2-dev/examples/control.c.gz
/usr/share/doc/libasound2-dev/examples/latency.c.gz
/usr/share/doc/libasound2-dev/examples/midifile.3.gz
/usr/share/doc/libasound2-dev/examples/midifile.c.gz
/usr/share/doc/libasound2-dev/examples/midifile.h
/usr/share/doc/libasound2-dev/examples/midiloop.c.gz
/usr/share/doc/libasound2-dev/examples/namehint.c
/usr/share/doc/libasound2-dev/examples/oldapi.c
/usr/share/doc/libasound2-dev/examples/pcm-multi-thread.c.gz
/usr/share/doc/libasound2-dev/examples/pcm.c.gz
/usr/share/doc/libasound2-dev/examples/pcm_min.c
/usr/share/doc/libasound2-dev/examples/playmidi1.c.gz
/usr/share/doc/libasound2-dev/examples/queue_timer.c
/usr/share/doc/libasound2-dev/examples/rawmidi.c.gz
/usr/share/doc/libasound2-dev/examples/seq-decoder.c.gz
/usr/share/doc/libasound2-dev/examples/seq-sender.c.gz
/usr/share/doc/libasound2-dev/examples/seq.c.gz
/usr/share/doc/libasound2-dev/examples/timer.c.gz
/usr/share/doc/libasound2-dev/examples/user-ctl-element-set.c.gz


link
---------------------------
https://github.com/justinlatimer/node-midi#readme

https://www.npmjs.com/package/midi-writer-js

https://github.com/mudcube/MIDI.js




La reconnaissance par le noyau
dmesg
[  224.960025] usb 2-3: new full speed USB device using ohci_hcd and address 3
[  225.169586] usb 2-3: configuration #1 chosen from 1 choice
[  225.236091] usbcore: registered new interface driver snd-usb-audio

[106730.152642] usb 2-1.6: USB disconnect, device number 6
[106732.171908] usb 2-1.6: new full-speed USB device number 7 using ehci-pci
[106732.283521] usb 2-1.6: New USB device found, idVendor=0944, idProduct=010d, bcdDevice= 1.00
[106732.283523] usb 2-1.6: New USB device strings: Mfr=1, Product=2, SerialNumber=0
[106732.283524] usb 2-1.6: Product: nanoKEY
[106732.283525] usb 2-1.6: Manufacturer: KORG INC.

phil@phil-OptiPlex-790:~$ cat /dev/midi1 
�2R�2@�0W�0@�7A�7@�<�<@�@�@@�Ao�A@�CZ�C@�=t�=@�:�:@�8r�8@�6%�6@�3B�3@�2=�2@�C�0F�HI�`L�xO�S�(V�@Y�X\�p_c� f�8i�Pl�ho�s�v�0y�H|�`��{�7v�Sq�ol�


phil@phil-OptiPlex-790:~/nodejs-files/midi/node-midi/test/input$ node /home/phil/nodejs-files/midi/node-midi/test/input/input-test.js 
2
nanoKEY:nanoKEY MIDI 1 20:0
m:176,25,127 d:0
m:176,25,0 d:0.256498544
m:176,25,127 d:1.053830082
m:176,25,0 d:0.134035864
m:176,21,127 d:0.32797481300000003
m:176,21,0 d:0.153037904
m:176,19,127 d:0.21598224700000002
m:176,19,0 d:0.103513348
m:176,18,127 d:0.250470507
m:176,18,0 d:0.10852959100000001
m:176,30,127 d:0.214455725
m:176,30,0 d:0.109039807
m:176,16,127 d:0.144501437
m:176,16,0 d:0.169461241
m:176,30,127 d:0.11704346600000001
m:176,30,0 d:0.095986451
m:176,21,127 d:0.6179905450000001
m:176,21,0 d:0.1230088
m:176,31,127 d:0.13488228700000002
m:176,31,0 d:0.12395881600000001
m:176,23,127 d:0.23916777300000003
m:176,23,0 d:0.11538202700000001
m:176,81,127 d:0.231448749
m:176,81,0 d:0.152524666
m:176,25,127 d:0.36599467100000005
m:176,25,0 d:0.09551835700000001
m:176,31,127 d:0.24798328200000003
m:176,31,0 d:0.17600084600000002
m:176,31,127 d:0.455455015
m:176,31,0 d:0.14904246100000001
m:176,30,127 d:0.570961099
m:176,30,0 d:0.148539464
m:176,28,127 d:0.22498537000000002
m:176,28,0 d:0.14835959


var midi = require("../../midi.js");

var input = new midi.Input();
console.log(input.getPortCount());
console.log(input.getPortName(1));
input.on('message', function(deltaTime, message) {
  console.log('m:' + message + ' d:' + deltaTime);
});
input.openPort(1);
setTimeout(function() {
  input.closePort();
}, 10000);

SEQUENCER
---------
https://github.com/rafaelcr/sequencer-pi

  318  npm install node-gyp
  319  npm install socket.io


  299  nano /home/phil/nodejs-files/midi/node-midi/test/input/input-test.js 
 nano /home/phil/nodejs-files/midi/sequencer-pi/node/midi1.js 
cp package.json /home/phil/nodejs-files/midi/sequencer-pi/

npm install


----
var express = require('express')
  , http = require('http');
//make sure you keep this order
var app = express();
var server = http.createServer(app);
var io = require('socket.io').listen(server);

//... 

server.listen(8000);

-----
Seq
----
phil@phil-OptiPlex-790:~/nodejs-files/midi/sequencer-pi/node$ cat midiold.js 
var app = require('http').createServer(httpHandler)
var io = require('socket.io').listen(app)
var fs = require('fs')
var midi = require('./build/Release/midi');

// HTTP web server will listen on port 8080 to avoid running as root.
app.listen(8080);
// The MIDI sequencer will communicate with the device on port 20 by default.
var sequence = new midi.Sequence(20);

// Simple web server implementation.
// Receives requests from socket.io and responds with the appropiate file from
// the web directory. This will only serve simple static pages, CSS
// and JS files.
function httpHandler(req, res) {
  var filename = (req.url == '/') ? 'index.html' : req.url;
  fs.readFile(__dirname + '/../web/' + filename,
  function (err, data) {
    if (err) {
      res.writeHead(500);
      return res.end('Error loading ' + filename);
    }
    res.writeHead(200);
    res.end(data);
  });
}

// Socket connection and message handlers.
io.sockets.on('connection', function(socket) {
  // Emit 'online' status when client is connected to acknowledge the channel.
  socket.emit('online', null);

  // Clear the sequencer when a new web session is initiated. Naturally, only
  // one sequencer can run at a time.
  socket.on('client_online', function(data) {
    console.log("Web sequencer online.");
    sequence.clear();
  });

  // Adds a note to the sequence.
  socket.on('note_add', function(data) {
    console.log("Adding note: " + data.note + " step: " + data.step);
    sequence.addNote(parseInt(data.note), parseInt(data.step));
  });

  // Removes a note from the sequence.
  socket.on('note_remove', function(data) {
    console.log("Removing note: " + data.note + " step: " + data.step);
    sequence.removeNote(parseInt(data.note), parseInt(data.step));
  });

  // Plays the sequence with the current configured MIDI notes.
  socket.on('play', function(data) {
    console.log("Playing sequence.");
    sequence.play();
  });

  // Stops playback.
  socket.on('stop', function(data) {
    console.log("Stopping sequence.");
    sequence.stop();
  });

  // Loops the current sequence and plays again.
  socket.on('loop', function(data) {
    sequence.stop();
    sequence.play();
  });
});

----------------------------

https://github.com/sksmatt/NodeJS-Ableton-Piano

https://github.com/wbajzek/arpeggiator/blob/master/arpeggiator.js

TONE ->
--------------
https://tonejs.github.io/docs/14.7.77/Clock

https://github.com/Ohjann/tonejs-sequencer.git
https://github.com/Ohjann/tonejs-sequencer


Sequencer 
https://www.npmjs.com/package/step-sequencer
https://github.com/freitagbr/step-sequencer


HOWLER
https://www.youtube.com/watch?v=jfNwB4tw8B0

#1 - https://www.youtube.com/watch?v=Aoru3iGDd8Q&list=PLXAhCH9FJ8zWm17RdQFAkdsghd8aKU_dq
https://github.com/musicandcode/Chord-Player/tree/master/src




JAVASCRITP STEP SEQ
https://github.com/mradambeck/javascript-step-sequencer

ERROR
----
phil@phil-OptiPlex-790:~/nodejs-files/javascript-step-sequencer$ node /home/phil/nodejs-files/javascript-step-sequencer/server.js
(node:753) DeprecationWarning: `open()` is deprecated in mongoose >= 4.11.0, use `openUri()` instead, or set the `useMongoClient` option if using `connect()` or `createConnection()`. See http://mongoosejs.com/docs/4.x/docs/connections.html#use-mongo-client
(Use `node --trace-deprecation ...` to show where the warning was created)
Server running on http://localhost:3000

events.js:292
      throw er; // Unhandled 'error' event
      ^
Error [MongoError]: failed to connect to server [localhost:27017] on first connect [Error: connect ECONNREFUSED 127.0.0.1:27017
    at TCPConnectWrap.afterConnect [as oncomplete] (net.js:1146:16) {
  name: 'MongoError'
}]
    at Pool.<anonymous> (/home/phil/nodejs-files/javascript-step-sequencer/node_modules/mongodb-core/lib/topologies/server.js:336:35)
    at Pool.emit (events.js:315:20)
    at Connection.<anonymous> (/home/phil/nodejs-files/javascript-step-sequencer/node_modules/mongodb-core/lib/connection/pool.js:280:12)
    at Object.onceWrapper (events.js:422:26)
    at Connection.emit (events.js:315:20)
    at Socket.<anonymous> (/home/phil/nodejs-files/javascript-step-sequencer/node_modules/mongodb-core/lib/connection/connection.js:189:49)
    at Object.onceWrapper (events.js:422:26)
    at Socket.emit (events.js:315:20)
    at emitErrorNT (internal/streams/destroy.js:106:8)
    at emitErrorCloseNT (internal/streams/destroy.js:74:3)
    at processTicksAndRejections (internal/process/task_queues.js:80:21)
Emitted 'error' event on NativeConnection instance at:
    at Immediate.<anonymous> (/home/phil/nodejs-files/javascript-step-sequencer/node_modules/mongoose/lib/connection.js:325:19)
    at processImmediate (internal/timers.js:461:21)

RESOLUTION
----------
https://peterthaleikis.com/posts/how-to-fix-throw-er-unhandled-error-event

rm -rf node_modules
rm package-lock.json yarn.lock
npm cache clear --force
npm install

Error [MongoError]: failed to connect to server [localhost:27017] 

http://doc.ubuntu-fr.org/mongodb



Remove Packages.
Remove any MongoDB packages that you had previously installed.

sudo apt-get purge mongodb-org*
3
Remove Data Directories.
Remove MongoDB databases and log files.

sudo rm -r /var/log/mongodb
sudo rm -r /var/lib/mongodb

https://www.mongodb.com/try/download/community

  513  sudo rm -r /var/log/mongodb
  514  sudo rm -r /var/lib/mongodb
  515  sudo dpkg -i mongodb-org-server_4.4.3_amd64.deb 


  534  sudo mkdir /var/lib/mongodb
  535  sudo mkdir /var/log/mongodb
  536  sudo chown -R mongodb:mongodb /var/lib/mongodb
  537  chown -R mongodb:mongodb /var/log/mongodb
  538  sudo chown -R mongodb:mongodb /var/log/mongodb
  539  sudo service mongod stop
  540  sudo service mongod start
  541  sudo systemctl status mongod
  542  history

http://127.0.0.1:27017/

It looks like you are trying to access MongoDB over HTTP on the native driver port.


phil@phil-OptiPlex-790:~/Téléchargements$ ls -l /var/lib/mongodb/
total 280
-rw------- 1 mongodb mongodb 20480 févr. 10 19:05 collection-0--878691929929129107.wt
-rw------- 1 mongodb mongodb 20480 févr. 10 19:05 collection-2--878691929929129107.wt
-rw------- 1 mongodb mongodb  4096 févr. 10 19:04 collection-4--878691929929129107.wt
-rw------- 1 mongodb mongodb  4096 févr. 10 19:26 collection-7--878691929929129107.wt
drwx------ 2 mongodb mongodb  4096 févr. 10 20:25 diagnostic.data
-rw------- 1 mongodb mongodb 20480 févr. 10 19:05 index-1--878691929929129107.wt
-rw------- 1 mongodb mongodb 20480 févr. 10 19:05 index-3--878691929929129107.wt
-rw------- 1 mongodb mongodb  4096 févr. 10 19:04 index-5--878691929929129107.wt
-rw------- 1 mongodb mongodb  4096 févr. 10 19:04 index-6--878691929929129107.wt
-rw------- 1 mongodb mongodb  4096 févr. 10 19:26 index-8--878691929929129107.wt
-rw------- 1 mongodb mongodb  4096 févr. 10 19:26 index-9--878691929929129107.wt
drwx------ 2 mongodb mongodb  4096 févr. 10 19:04 journal
-rw------- 1 mongodb mongodb 36864 févr. 10 19:27 _mdb_catalog.wt
-rw------- 1 mongodb mongodb     5 févr. 10 19:04 mongod.lock
-rw------- 1 mongodb mongodb 36864 févr. 10 19:28 sizeStorer.wt
-rw------- 1 mongodb mongodb   114 févr. 10 19:04 storage.bson
-rw------- 1 mongodb mongodb    47 févr. 10 19:04 WiredTiger
-rw------- 1 mongodb mongodb  4096 févr. 10 19:04 WiredTigerHS.wt
-rw------- 1 mongodb mongodb    21 févr. 10 19:04 WiredTiger.lock
-rw------- 1 mongodb mongodb  1255 févr. 10 20:25 WiredTiger.turtle
-rw------- 1 mongodb mongodb 69632 févr. 10 20:25 WiredTiger.wt



  486  apt --fix-broken install mongod
  487  sudo dpkg -i --force-overwrite /var/cache/apt/archives/
  488  sudo dpkg -i --force-overwrite  /var/cache/apt/archives/mongodb-database-tools_100.3.0-1-g8b223b0a
  489  sudo apt-get autoremove --purge -y
  490  [[ $(apt-mark showmanual | grep -E "linux-.*[0-9]" | grep -v "hwe") != '' ]] && apt-mark showmanual | grep -E "linux-.*[0-9]" | grep -v "hwe" | xargs sudo apt-mark auto
  491  sudo apt-get autoremove --purge -y
  492  dpkg -i --force-overwrite 
  493  sudo dpkg -i --force-overwrite 
  494  sudo dpkg -i mongodb-org-server_4.4.3_amd64.deb 
  495  sudo dpkg -i --force-overwrite mongodb-org-server_4.4.3_amd64.deb 
  496  sudo mongod service starty
  497  sudo mongod service start
  498  sudo mongod
  499  sudo mongod service start
  500  sudo systemctl start mongod
  501  sudo mongod
  502  sudo systemctl status mongod
  503  sudo systemctl start mongod
  504  sudo systemctl status mongod
  505  sudo systemctl enable mongod
  506  sudo systemctl status mongod
  507  sudo systemctl start mongod
  508  sudo systemctl status mongod
  509  cat /var/log/mongodb/mongod.log
  510  sudo cat /var/log/mongodb/mongod.log
  511  mongo
  512  sudo apt-get purge mongodb-org*
  513  sudo rm -r /var/log/mongodb
  514  sudo rm -r /var/lib/mongodb
  515  sudo dpkg -i mongodb-org-server_4.4.3_amd64.deb 
  516  sudo systemctl start mongod
  517  sudo systemctl status mongod
  518  sudo systemctl enable mongod
  519  sudo systemctl stop mongod
  520  sudo systemctl start mongod
  521  sudo systemctl status mongod
  522  sudo apt-get purge mongodb-org*
  523  sudo rm -r /var/log/mongodb
  524  sudo rm -r /var/lib/mongodb
  525  sudo apt-get install -y mongodb-org
  526  sudo systemctl daemon-reload
  527  sudo systemctl start mongod
  528  sudo systemctl status mongod
  529  chown -R mongodb:mongodb /var/lib/mongodb
  530  chown mongodb:mongodb /tmp/mongodb-27017.sock
  531  sudo rm -rf /tmp/mongodb-27017.sock
  532  sudo service mongod start
  533  sudo systemctl status mongod
  534  sudo mkdir /var/lib/mongodb
  535  sudo mkdir /var/log/mongodb
  536  sudo chown -R mongodb:mongodb /var/lib/mongodb
  537  chown -R mongodb:mongodb /var/log/mongodb
  538  sudo chown -R mongodb:mongodb /var/log/mongodb
  539  sudo service mongod stop
  540  sudo service mongod start
  541  sudo systemctl status mongod
  542  history
  543  ls /var/lib/mongodb/
  544  ls -l /var/lib/mongodb/
  545  nano /var/lib/mongodb/WiredTiger.turtle 
  546  sudo nano /var/lib/mongodb/WiredTiger.turtle 
  547  ls -l /var/lib/mongodb/
  548  sudo apt install guvcview 
  549  sudo apt --fix-broken install
  550  sudo apt -f --fix-broken install
  551  sudo apt install guvcview 
  552  history



 
