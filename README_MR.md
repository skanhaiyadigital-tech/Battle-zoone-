# BATTLE ZONE INDIA — Unity Android Starter Project

हा Unity Android प्रोजेक्टचा **खेळता येण्याजोगा बेस/Starter scaffold** आहे. हा अजून पूर्ण 50-player online गेम नाही. 50-player multiplayer साठी Photon Fusion किंवा dedicated authoritative server, matchmaking, backend, testing आणि server deployment जोडणे आवश्यक आहे.

## ठरलेली गेम दिशा
- नाव: BATTLE ZONE INDIA
- प्लॅटफॉर्म: Android
- Engine: Unity 2022.3 LTS
- Camera: Third Person
- Match target: 50 players
- मुख्य वातावरण: Indian Village + City
- प्रकार: Battle Royale

## सध्या समाविष्ट C# systems
- Third-person character movement, sprint आणि jump
- Third-person follow camera व look input bridge
- Health / damage / heal
- Raycast weapon, magazine आणि reload
- Safe-zone shrink logic
- Match manager prototype (50-player count placeholder)
- Mobile UI button bridge

## Unity मध्ये उघडण्याची पद्धत
1. Unity Hub मध्ये **Add > Add project from disk** निवडा.
2. या ZIP मधून extract केलेला `BATTLE_ZONE_INDIA_Unity_Android` फोल्डर निवडा.
3. Unity 2022.3 LTS चा installed patch वापरा. `ProjectSettings/ProjectVersion.txt` मधील `2022.3.XXf1` ही placeholder नोंद तुमच्या installed 2022.3 patch ने बदला किंवा Unity Hub ला project upgrade करू द्या.
4. नवीन Scene तयार करा आणि `Assets/Scenes` मध्ये `Main.unity` नावाने save करा.
5. Player GameObject तयार करा; त्यावर CharacterController, ThirdPersonPlayer आणि Health जोडा. Camera ला ThirdPersonCamera जोडा आणि `target` मध्ये Player द्या. Player script च्या `cameraTransform` मध्ये Main Camera द्या.
6. Weapon object वर Weapon script जोडा आणि `aimCamera` मध्ये Main Camera द्या.
7. UI Buttons/Joystick च्या OnClick किंवा तुमच्या joystick package मधून `MobileInputBridge` methods जोडा.
8. Build Settings > Android > Switch Platform करा. Player Settings मध्ये Package Identifier उदा. `com.yourstudio.battlezoneindia` सेट करा.

## महत्त्वाच्या पुढील कामांच्या नोंदी
- Multiplayer: Photon Fusion/इतर networking SDK, server authority, 50-player load test आणि matchmaking
- Lobby: Solo/Duo/Squad, Room ID/password, friends/invites
- Game modes: Casual/Ranked, Clash Arena, Training, Custom Room; पुढे Zombie/Tournament
- Gameplay: loot, inventory, guns/scopes/attachments, parachute/drop, vehicles, emotes, skins/bundles, revive आणि spectator
- Maps: Desi Village + City हे पहिले map; नंतर Island X, Desert Storm, Snow Valley, Jungle War, Port City
- Backend: account/profile, stats, ranks, friends, purchases आणि cloud save
- Voice chat, anti-cheat, analytics, optimization आणि Google Play release pipeline

## लक्षात ठेवा
या ZIP मध्ये वास्तविक 3D models, textures, finished scenes, animations, sound effects, matchmaking server किंवा production multiplayer service समाविष्ट नाहीत. ते वेगळे तयार/जोडावे लागतील. या starter code ला production-ready किंवा 50-player online tested समजू नका.
