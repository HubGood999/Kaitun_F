local v0=string.char;local v1=string.byte;local v2=string.sub;local v3=bit32 or bit ;local v4=v3.bxor;local v5=table.concat;local v6=table.insert;local function v7(v91,v92) local v93={};for v127=1, #v91 do v6(v93,v0(v4(v1(v2(v91,v127,v127 + 1 )),v1(v2(v92,1 + (v127% #v92) ,1 + (v127% #v92) + 1 )))%256 ));end return v5(v93);end local v8=game:GetService(v7("\253\202\220\45\242\178\201\25","\126\177\163\187\69\134\219\167"));local v9=true;local function v10(v94) local v95,v96,v97=v94:match(v7("\107\136\46\142\181\121\133\111\193\183\106\151\98\128\248\104\132","\156\67\173\74\165"));return (tonumber(v95) * 3600) + (tonumber(v96) * (232 -172)) + tonumber(v97) ;end if (getgenv().Setting[v7("\18\182\91\27","\38\84\215\41\118\220\70")][v7("\99\19\54\6\247\94\17","\158\48\118\66\114")][v7("\141\20\35\118\81\170\244\184\48\21\36","\155\203\68\112\86\19\197")]==true) then local v128=game;local v129=v128.Workspace;local v130=v128.Lighting;local v131=v129.Terrain;v131.WaterWaveSize=0;v131.WaterWaveSpeed=1128 -(307 + 821) ;v131.WaterReflectance=0;v131.WaterTransparency=0;v130.GlobalShadows=false;v130.FogEnd=math.huge;v130.Brightness=0 -0 ;for v142,v143 in ipairs(v129:GetDescendants()) do if (v143:IsA(v7("\118\220\36\232","\152\38\189\86\156\32\24\133")) or v143:IsA(v7("\201\89\174\73\242","\38\156\55\199")) or v143:IsA(v7("\139\114\110\38\22\102\205\70\172\122\121\24\18\102\238","\35\200\29\28\72\115\20\154")) or v143:IsA(v7("\45\173\196\204\158\28\53\11\171","\84\121\223\177\191\237\76"))) then v143.Material=Enum.Material.Plastic;v143.Reflectance=1812 -(1293 + 519) ;elseif (v143:IsA(v7("\159\83\202\161\54","\161\219\54\169\192\90\48\80")) or v143:IsA(v7("\125\71\24\49\92\80\5","\69\41\34\96"))) then v143.Transparency=1 -0 ;elseif (v143:IsA(v7("\140\194\197\30\11\40\176\198\242\7\11\63\168\198\197","\75\220\163\183\106\98")) or v143:IsA(v7("\54\168\138\62\213","\185\98\218\235\87"))) then v143.Lifetime=NumberRange.new(0);elseif v143:IsA(v7("\238\36\55\234\209\185\194\51\41","\202\171\92\71\134\190")) then local v234=0 -0 ;while true do if (v234==0) then v143.BlastPressure=1 -0 ;v143.BlastRadius=4 -3 ;break;end end elseif (v143:IsA(v7("\15\200\62\141","\232\73\161\76")) or v143:IsA(v7("\136\201\77\73\50\178\222\74\73","\126\219\185\34\61")) or v143:IsA(v7("\63\195\81\121\123","\135\108\174\62\18\30\23\147")) or v143:IsA(v7("\133\249\43\217\19\162\54\212","\167\214\137\74\171\120\206\83"))) then v143.Enabled=false;elseif v143:IsA(v7("\166\245\33\85\200\166\153\228","\199\235\144\82\61\152")) then local v266=0 -0 ;while true do if (v266==1) then v143.TextureID=v7("\86\70\234\115\82\79\233\121\80\67\225\124\85\78\224\126\80","\75\103\118\217");break;end if (v266==(0 + 0)) then v143.Material=Enum.Material.Plastic;v143.Reflectance=0 + 0 ;v266=2 -1 ;end end end end for v144,v145 in ipairs(v130:GetChildren()) do if (v145:IsA(v7("\229\88\101\6\156\24\193\81\115\0","\126\167\52\16\116\217")) or v145:IsA(v7("\251\59\46\178\181\0\239\237\40\38\133\183\13","\156\168\78\64\224\212\121")) or v145:IsA(v7("\36\225\169\193\21\205\170\220\21\235\166\218\14\225\171\235\1\232\160\205\19","\174\103\142\197")) or v145:IsA(v7("\116\36\80\55\40\123\254\80\45\92\44","\152\54\72\63\88\69\62")) or v145:IsA(v7("\240\193\254\72\220\235\232\122\221\193\226\88\241\194\232\89\215\208","\60\180\164\142"))) then v145.Enabled=false;end end end local v11=false;local v12=true;local v13=false;local v14=false;local v15=false;local v16=game:GetService(v7("\106\91\21\37\46\238\19\76\91\1\26\51\226\0\89\89\0","\114\56\62\101\73\71\141"));function Equip_Rods(v98) pcall(function() local v140=0;local v141;while true do if (v140==(0 + 0)) then v141=game:GetService(v7("\136\229\218\221\189\251\200","\164\216\137\187")).LocalPlayer.Backpack;for v201,v202 in pairs(v141:GetChildren()) do if (v202:IsA(v7("\230\233\62\190","\107\178\134\81\210\198\158")) and (v202.ToolTip==v98)) then game:GetService(v7("\8\2\131\223\175\42\29","\202\88\110\226\166")).LocalPlayer.Character.Humanoid:EquipTool(v202);end end break;end end end);end function bar() game.Players.LocalPlayer.PlayerGui.reel.bar.playerbar.Position=game.Players.LocalPlayer.PlayerGui.reel.bar.fish.Position;end function SendKeyEvent(v101) local v102=0 + 0 ;while true do if (0==v102) then game:service(v7("\245\6\144\227\223\194\3\171\249\218\214\27\175\246\196\194\8\135\229","\170\163\111\226\151")):SendKeyEvent(true,v101,false,game);game:service(v7("\39\57\160\44\91\54\37\56\62\162\45\90\26\40\31\49\181\61\92","\73\113\80\210\88\46\87")):SendKeyEvent(false,v101,false,game);break;end end end function farmCoins() local v103=game.Players.LocalPlayer;if  not v103:FindFirstChild(v7("\177\32\204\11\226\147\11\216\27","\135\225\76\173\114")):FindFirstChild(v7("\9\229\185\187\169\168\174","\199\122\141\216\208\204\221")) then local v146=0;local v147;while true do if (v146==(0 + 0)) then v147=0;while true do if (v147==(1096 -(709 + 387))) then Equip_Rods(v7("\171\212\3\243\112","\150\205\189\112\144\24"));game:GetService(v7("\23\129\175\64\13\139\16\4\32\128\140\88\11\154\16\23\32","\112\69\228\223\44\100\232\113")):WaitForChild(v7("\209\9\2\221\162\111","\230\180\127\103\179\214\28")):WaitForChild(v7("\191\0\83\74\197\77\236","\128\236\101\63\38\132\33")):InvokeServer();v147=1859 -(673 + 1185) ;end if ((2 -1)==v147) then for v232,v233 in pairs(v103.Character:GetChildren()) do if (v233:IsA(v7("\129\166\21\65\186","\175\204\201\113\36\214\139")) or v233:IsA(v7("\115\195\58\208","\100\39\172\85\188")) or v233:IsA(v7("\157\121\171\148","\83\205\24\217\224"))) then local v240=v233:FindFirstChild(v7("\227\211\200\51\242\214","\93\134\165\173"));if (v240 and v240:FindFirstChild(v7("\189\243\210\214","\30\222\146\161\162\90\174\210")) and string.find(v233.Name,v7("\215\65\116","\106\133\46\16"))) then v240.cast:FireServer(321 -221 ,1 -0 );wait(0.25);break;end end end break;end end break;end end else local v148=0 + 0 ;while true do if (v148==(0 + 0)) then game:GetService(v7("\127\53\122\207\95\82\78\41\112\249","\32\56\64\19\156\58")).SelectedCoreObject=v103:WaitForChild(v7("\106\196\228\79\95\224\167\79\193","\224\58\168\133\54\58\146")):WaitForChild(v7("\74\94\74\246\112\147\142","\107\57\54\43\157\21\230\231")).safezone:FindFirstChild(v7("\217\158\5\225\182\210","\175\187\235\113\149\217\188"));game:GetService(v7("\10\166\147\88\246\120\116\21\161\145\89\247\84\121\50\174\134\73\241","\24\92\207\225\44\131\25")):SendKeyEvent(true,Enum.KeyCode.Return,false,game);v148=1;end if (v148==1) then game:GetService(v7("\125\218\170\88\14\124\71\250\182\92\14\105\102\210\182\77\28\120\89","\29\43\179\216\44\123")):SendKeyEvent(false,Enum.KeyCode.Return,false,game);bar();break;end end end end function buyRod(v104,v105) local v106=0;local v107;while true do if (v106==(1 -0)) then v107.Character.HumanoidRootPart.CFrame=v104;game.Workspace.CurrentCamera.CFrame=CFrame.lookAt(game.Workspace.CurrentCamera.CFrame.Position,v105);v106=1 + 1 ;end if (v106==(3 -1)) then SendKeyEvent("E");wait(1);v106=5 -2 ;end if (v106==(1883 -(446 + 1434))) then if v107.PlayerGui.over:FindFirstChild(v7("\173\203\47\65\173\205","\44\221\185\64")) then for v215,v216 in pairs({v7("\44\232\93\76\118\35\242\92\75\124\15\182\107\83\122\2\236","\19\97\135\40\63")}) do for v220,v221 in pairs(getconnections(v107.PlayerGui.over.prompt.confirm[v216])) do v221.Function();end end end break;end if (v106==(0 -0)) then v107=game.Players.LocalPlayer;wait(1848 -(559 + 1288) );v106=1;end end end function Click_Buy() if game.Players.LocalPlayer.PlayerGui.over:FindFirstChild(v7("\190\78\60\54\63\37","\81\206\60\83\91\79")) then for v168,v169 in pairs({v7("\99\164\197\97\42\225\88\176\90\164\222\35\12\207\68\167\69","\196\46\203\176\18\79\163\45")}) do for v197,v198 in pairs(getconnections(game.Players.LocalPlayer.PlayerGui.over.prompt.confirm[v169])) do v198.Function();end end else for v170,v171 in ipairs(workspace:GetDescendants()) do if v171:IsA(v7("\136\48\113\6\45\246\230\172\59\78\12\43\246\255\172","\143\216\66\30\126\68\155")) then local v204=0;local v205;while true do if (v204==(1931 -(609 + 1322))) then v205=454 -(13 + 441) ;while true do if (v205==(0 -0)) then v171.HoldDuration=0 -0 ;v171.MaxActivationDistance=498 -398 ;break;end end break;end end end end SendKeyEvent("E");wait(0.5 + 0 );if game.Players.LocalPlayer.PlayerGui.over:FindFirstChild(v7("\186\218\2\198\213\183","\129\202\168\109\171\165\195\183")) then for v206,v207 in pairs({v7("\15\87\34\203\219\54\243\54\76\56\214\143\55\234\43\91\60","\134\66\56\87\184\190\116")}) do for v217,v218 in pairs(getconnections(game.Players.LocalPlayer.PlayerGui.over.prompt.confirm[v207])) do v218.Function();end end else SendKeyEvent("E");end end end function buyRodV_2(v108,v109) local v110=game.Players.LocalPlayer;local v111=v110.Character or v110.CharacterAdded:Wait() ;local v112=v111:WaitForChild(v7("\20\36\4\186\23\228\40\49\14\62\6\175\41\234\51\33","\85\92\81\105\219\121\139\65"));v112.CFrame=CFrame.new(v108);local v114=game.Workspace.CurrentCamera;v114.CFrame=CFrame.lookAt(v114.CFrame.Position,v109);SendKeyEvent("E");wait(1 + 0 );if v110.PlayerGui.over:FindFirstChild(v7("\237\161\95\72\108\203","\191\157\211\48\37\28")) then for v172,v173 in pairs({v7("\242\16\225\15\63\253\10\224\8\53\209\78\215\16\51\220\20","\90\191\127\148\124")}) do for v199,v200 in pairs(getconnections(v110.PlayerGui.over.prompt.confirm[v173])) do v200.Function();end end end end local v16=game:GetService(v7("\74\130\62\27\113\132\47\3\125\131\29\3\119\149\47\16\125","\119\24\231\78"));local v17=game:GetService(v7("\178\33\164\83\217\82\2","\113\226\77\197\42\188\32"));local v18=v17.LocalPlayer;local v19=Instance.new(v7("\9\21\230\176\63\24\211\160\51","\213\90\118\148"));v19.Parent=v18:WaitForChild(v7("\107\34\181\79\72\73\9\161\95","\45\59\78\212\54"));v19.ZIndexBehavior=Enum.ZIndexBehavior.Sibling;local v23=Instance.new(v7("\54\68\130\134\131","\144\112\54\227\235\230\78\205"));v23.Parent=v19;v23.AnchorPoint=Vector2.new(0.5 -0 ,0.5);v23.BackgroundColor3=Color3.fromRGB(49 + 40 ,163 -74 ,59 + 30 );v23.BackgroundTransparency=0.5;v23.BorderSizePixel=0 + 0 ;v23.Position=UDim2.new(0.5 + 0 ,0 + 0 ,0.5 + 0 ,433 -(153 + 280) );v23.Size=UDim2.new(0,1155 -755 ,0 + 0 ,198 + 302 );v23.Visible=true;local v32=Instance.new(v7("\134\1\44\243\194\85\182\58","\59\211\72\111\156\176"));v32.CornerRadius=UDim.new(0,11 + 9 );v32.Parent=v23;local v35=Instance.new(v7("\103\138\226\42\75\165\246\57\90\136\237","\77\46\231\131"));v35.Parent=v23;v35.AnchorPoint=Vector2.new(0.5,0.5 + 0 );v35.BackgroundTransparency=1;v35.Size=UDim2.new(0 + 0 ,304 -104 ,0 + 0 ,150);v35.Position=UDim2.new(0.5,667 -(89 + 578) ,0.1 + 0 ,0 -0 );v35.Image=v7("\178\64\162\80\224\27\249\87\173\67\248\82\181\86\186\79\162\26\181\79\183\27\183\83\169\81\162\15\229\93\178\29\235\4\226\20\232\1\225\19\232\0\239\24\238\1\239","\32\218\52\214");local v42=Instance.new(v7("\123\62\18\167\227\190\64\72","\58\46\119\81\200\145\208\37"));v42.CornerRadius=UDim.new(1049 -(572 + 477) ,3 + 12 );v42.Parent=v35;local v45=Instance.new(v7("\30\165\28\165\186\169\26\42\149\63\185\189","\86\75\236\80\204\201\221"));v45.Parent=v23;v45.SortOrder=Enum.SortOrder.LayoutOrder;v45.Padding=UDim.new(0 + 0 ,2 + 8 );local function v50(v116,v117,v118,v119) local v120=0;local v121;while true do if (v120==(89 -(84 + 2))) then v121.Text=v117;v121.TextColor3=v119 or Color3.fromRGB(420 -165 ,255,184 + 71 ) ;v120=846 -(497 + 345) ;end if (v120==1) then v121.AnchorPoint=Vector2.new(0.5,0.5 + 0 );v121.BackgroundTransparency=1 + 0 ;v120=1335 -(605 + 728) ;end if (v120==(0 + 0)) then v121=Instance.new(v7("\70\68\111\145\210\138\112\68\123","\235\18\33\23\229\158"));v121.Parent=v116;v120=1;end if (v120==4) then v121.TextSize=v118;return v121;end if (v120==2) then v121.Size=UDim2.new(1 -0 ,0 + 0 ,0 -0 ,37 + 3 );v121.Font=Enum.Font.FredokaOne;v120=7 -4 ;end end end v50(v23,v7("\126\191\217\174\67\250\233\174\82","\219\48\218\161"),31 + 9 ,Color3.fromRGB(16,157,668 -(457 + 32) ));v50(v23,v7("\172\49\93\92\207\64\160\207\112\117\93\206\65\160\173","\128\132\17\28\41\187\47"),20);local v51=v50(v23,v7("\50\38\7\46\72\18\114\92\122\113\14\51\2\51\83\6\124\72\116","\61\97\82\102\90"),11 + 14 );local v52=Instance.new(v7("\138\60\170\70\194","\105\204\78\203\43\167\55\126"));v52.Parent=v19;v52.AnchorPoint=Vector2.new(0.5,1402.5 -(832 + 570) );v52.BackgroundColor3=Color3.fromRGB(84 + 5 ,24 + 65 ,314 -225 );v52.BackgroundTransparency=0.5;v52.BorderSizePixel=0 + 0 ;v52.Position=UDim2.new(0.5,796 -(588 + 208) ,0.5,0 -0 );v52.Size=UDim2.new(0.6,1800 -(884 + 916) ,0.5 -0 ,0 + 0 );v52.Visible=false;local v61=Instance.new(v7("\144\131\0\17\1\10\194\67","\49\197\202\67\126\115\100\167"));v61.CornerRadius=UDim.new(0,20);v61.Parent=v52;local v64=Instance.new(v7("\2\114\243\32\147\66\114\54\66\208\60\148","\62\87\59\191\73\224\54"));v64.Parent=v52;v64.SortOrder=Enum.SortOrder.LayoutOrder;v64.Padding=UDim.new(0,663 -(232 + 421) );local v68=Instance.new(v7("\193\16\251\196\226","\169\135\98\154"));v68.Parent=v52;v68.BackgroundTransparency=1890 -(1569 + 320) ;v68.Size=UDim2.new(1 + 0 ,0 + 0 ,0.8,0 -0 );v68.LayoutOrder=608 -(316 + 289) ;local v73=Instance.new(v7("\254\94\3\70\244\55\228\202\110\43\65\233","\168\171\23\68\52\157\83"));v73.Parent=v68;v73.CellSize=UDim2.new(0.23,0 -0 ,0,2 + 38 );v73.CellPadding=UDim2.new(1453.02 -(666 + 787) ,0,425.02 -(360 + 65) ,0 + 0 );local v77={v7("\192\99\244\164\43\36\137\243\49\199\162\33","\231\148\17\149\205\69\77"),v7("\176\171\198\232\67\246\131\231\245\244\83","\159\224\199\167\155\55"),v7("\212\242\46\208\248\253\124\224\248\247","\178\151\147\92"),v7("\170\252\95\38\82\126\117\136","\26\236\157\44\82\114\44"),v7("\6\33\219\92\106\28\218\95","\59\74\78\181"),v7("\9\196\89\81\170\101\227\85\94","\211\69\177\58\58"),v7("\133\228\105\252\237\139\133\234\125","\171\215\133\25\149\137"),v7("\210\220\55\251\235\41\188\112\238\204","\34\129\168\82\154\143\80\156"),v7("\163\189\33\31\93\64\140\197\128\60\15","\233\229\210\83\107\40\46"),v7("\236\67\53\216\0\213\2\0\217\1","\101\161\34\82\182"),v7("\220\31\80\250\222\236\150\110\218\2\93","\78\136\109\57\158\187\130\226")};local v78={};for v122,v123 in ipairs(v77) do local v124=0 + 0 ;local v125;while true do if (v124==(0 -0)) then v125=v50(v68,v123   .. " : ❌" ,4 + 21 );v78[v123]=v125;break;end end end local v79=Instance.new(v7("\23\50\248\246\59\29\236\229\42\48\247","\145\94\95\153"));v79.Parent=v52;v79.Size=UDim2.new(0,228 -128 ,0,75 + 10 );v79.Position=UDim2.new(0.5,0 + 0 ,0.9 -0 ,0 + 0 );v79.AnchorPoint=Vector2.new(0.5,0);v79.BackgroundTransparency=1;v79.Image=v7("\245\217\0\197\20\248\178\218\3\194\0\165\242\207\24\218\86\249\254\194\25\154\79\164\238\200\0\154\17\190\249\144\69\133\26\227\175\152\67\134\28\227\164\149\64\128\23","\215\157\173\116\181\46");local v86=Instance.new(v7("\0\157\168\253\200\59\177\153","\186\85\212\235\146"));v86.CornerRadius=UDim.new(0 -0 ,1259 -(485 + 759) );v86.Parent=v79;local function v89() local v126=0;while true do if (0==v126) then v23.Visible= not v23.Visible;v52.Visible= not v52.Visible;break;end end end v35.MouseButton1Click:Connect(v89);v79.MouseButton1Click:Connect(v89);spawn(function() while task.wait(0) do pcall(function() local v149=0 -0 ;local v150;while true do if (v149==(1189 -(442 + 747))) then v150=v16.playerstats[v18.Name]:FindFirstChild(v7("\240\142\18\237","\56\162\225\118\158\89\142"));if v150 then for v225,v226 in ipairs(v77) do if v150:FindFirstChild(v226) then v78[v226].Text=v226   .. " ✅" ;else v78[v226].Text=v226   .. " ❌" ;end end end break;end end end);end end);local v90=v50(v23,v7("\20\69\236\170\52\221\80\69\154\239\14\215\93\1\201\161\37\150\18\75\128\230","\184\60\101\160\207\66"),30);spawn(function() while task.wait() do pcall(function() v90.Text=v7("\121\194\80\185\39\135\112\252\107\194","\220\81\226\28")   .. game:GetService(v7("\33\208\146\247\227\196\18\193\135\255\217\211\28\199\131\252\239","\167\115\181\226\155\138")).playerstats[v18.Name].Stats.level.Value   .. v7("\162\62\167\127\116\120\200\241\98\189\28","\166\130\66\135\60\27\17")   .. game:GetService(v7("\118\79\222\121\57\71\75\218\112\52\119\94\193\103\49\67\79","\80\36\42\174\21")).playerstats[v18.Name].Stats.coins.Value   .. v7("\14\89","\26\46\112\87") ;end);end end);spawn(function() while task.wait() do pcall(function() bar();end);end end);spawn(function() while task.wait() do pcall(function() local v152=1135 -(832 + 303) ;local v153;while true do if (v152==(946 -(88 + 858))) then v153=v16.playerstats[game.Players.LocalPlayer.Name]:FindFirstChild(v7("\139\44\175\103","\212\217\67\203\20\223\223\37"));if v153:FindFirstChild(v7("\142\159\161\214\191\131\188\146\136\130\172","\178\218\237\200")) then game:GetService(v7("\132\176\246\220\191\182\231\196\179\177\213\196\185\167\231\215\179","\176\214\213\134")):WaitForChild(v7("\228\172\181\223\169\81\92\231","\57\148\205\214\180\200\54")):WaitForChild(v7("\60\248\33","\22\114\157\85\84")):WaitForChild(v7("\246\238\92\246\82\242\231\225\218\6\205\77","\200\164\171\115\164\61\150")):FireServer(v7("\138\230\10\65\134\176\224\67\119\140\186","\227\222\148\99\37"));elseif v153:FindFirstChild(v7("\1\83\66\255\253\115\96\93\242","\153\83\50\50\150")) then game:GetService(v7("\111\115\99\16\122\168\76\73\115\119\47\103\164\95\92\113\118","\45\61\22\19\124\19\203")):WaitForChild(v7("\209\19\14\254\3\119\188\210","\217\161\114\109\149\98\16")):WaitForChild(v7("\60\37\44","\20\114\64\88\28\220")):WaitForChild(v7("\3\36\157\134\247\212\242\20\16\199\189\232","\221\81\97\178\212\152\176")):FireServer(v7("\255\230\13\242\30\141\213\18\255","\122\173\135\125\155"));end break;end end end);end end);spawn(function() while task.wait() do pcall(function() local v154={[v7("\182\192\16\176\59\113\250\139\197","\168\228\161\96\217\95\81")]={C=14000,[v7("\249\238\13","\55\187\177\78\60\79")]=CFrame.new( -(460 + 1049),118 + 24 ,761),[v7("\11\241\124","\224\77\174\63\139\38\175")]=CFrame.new( -(159 + 3684),133,1128 -(766 + 23) )},[v7("\176\83\89\39\138\72\86\41\196\115\87\42","\78\228\33\56")]={C=1481 -1181 ,[v7("\236\65\145","\229\174\30\210\99")]=CFrame.new(625 -167 ,151,608 -377 ),[v7("\61\210\165","\89\123\141\230\49\141\93")]=CFrame.new( -(13043 -9200),133,339)},[v7("\195\125\247\31\4\67\240\49\196\3\20","\42\147\17\150\108\112")]={C=1973 -(1036 + 37) ,[v7("\45\153\14","\136\111\198\77\31\135")]=CFrame.new(455,108 + 43 ,230),[v7("\36\54\132","\201\98\105\199\54\221\132\119")]=CFrame.new( -(7483 -3640),105 + 28 ,339)},[v7("\154\13\145\35\13\59\236\139\3\135","\204\217\108\227\65\98\85")]={C=3480 -(641 + 839) ,[v7("\124\252\214","\160\62\163\149\133\76")]=CFrame.new(1366 -(910 + 3) ,389 -236 ,224),[v7("\240\159\46","\163\182\192\109\79")]=CFrame.new( -(5527 -(1466 + 218)),133,339)},[v7("\18\39\19\212\181\6\41\4","\149\84\70\96\160")]={C=2069 + 2431 ,[v7("\26\57\46","\141\88\102\109")]=CFrame.new(1596 -(556 + 592) ,54 + 97 ,1028 -(329 + 479) ),[v7("\149\108\233","\161\211\51\170\16\122\93\53")]=CFrame.new( -(4697 -(174 + 680)),133,1164 -825 )},[v7("\215\161\188\47\187\156\189\44","\72\155\206\210")]={C=4500,[v7("\100\69\119","\83\38\26\52\110")]=CFrame.new(1006 -520 ,175,146),[v7("\126\40\4","\38\56\119\71")]=CFrame.new( -(2744 + 1099),872 -(396 + 343) ,339)},[v7("\223\250\91\221\60\22\193\224\92","\54\147\143\56\182\69")]={C=465 + 4785 ,[v7("\244\190\220","\191\182\225\159\41")]=CFrame.new(1922 -(29 + 1448) ,151,222),[v7("\13\45\11","\162\75\114\72\53\235\231")]=CFrame.new( -3843,1522 -(135 + 1254) ,1276 -937 )},[v7("\191\40\65\227\87\27\204\14\75\230","\98\236\92\36\130\51")]={C=32683 -25683 ,[v7("\134\38\47","\80\196\121\108\218\37\200\213")]=CFrame.new( -(1007 + 504),1670 -(389 + 1138) ,1333 -(102 + 472) ),[v7("\38\76\33","\234\96\19\98\31\43\110")]=CFrame.new( -(3627 + 216),133,188 + 151 )},[v7("\32\16\64\211\185\124\142\70\45\93\195","\235\102\127\50\167\204\18")]={C=11889 + 861 ,[v7("\114\158\214","\78\48\193\149\67\36")]=CFrame.new( -(3068 -(320 + 1225)),255 -111 ,771),[v7("\22\33\163","\33\80\126\224\120")]=CFrame.new( -3843,82 + 51 ,339)},[v7("\193\169\4\202\89\248\232\49\203\88","\60\140\200\99\164")]={C=16464 -(157 + 1307) ,[v7("\165\203\39","\194\231\148\100\70")]=CFrame.new( -(2054 -(821 + 1038)),133,4817 -2886 ),[v7("\96\115\226","\168\38\44\161\195\150")]=CFrame.new( -(421 + 3422),133,339)}};local v155=true;for v186,v187 in pairs(v154) do if  not game.ReplicatedStorage.playerstats[game.Players.LocalPlayer.Name].Rods:FindFirstChild(v186) then v155=false;break;end end if v155 then v11=true;v15=true;return;end for v188,v189 in pairs(v154) do if (getgenv().Setting[v7("\166\253\144\123","\118\224\156\226\22\80\136\214")][v7("\108\225\75\141\67\226\25\178\77\234","\224\34\142\57")][v188] and  not game.ReplicatedStorage.playerstats[game.Players.LocalPlayer.Name].Rods:FindFirstChild(v188)) then local v208=0 -0 ;local v209;local v210;while true do local v219=0 + 0 ;while true do if (0==v219) then if (v208==1) then local v243=0;while true do if (v243==0) then if (v210<v189.C) then local v271=0 -0 ;local v272;while true do if (v271==(1026 -(834 + 192))) then v272=0 + 0 ;while true do if (v272==(1 + 0)) then farmCoins();break;end if (v272==0) then game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame=v189.F_C;v51.Text=v7("\252\234\101\229\130\201\221\171\116\231\130\201\201\171\99\231\203\197\207\242\55","\167\186\139\23\136\235")   .. v188 ;v272=1 + 0 ;end end break;end end else local v273=0 -0 ;local v274;while true do if (v273==0) then v274=304 -(300 + 4) ;while true do if (v274==(0 + 0)) then v51.Text=v7("\56\160\145\4\20\178\200","\109\122\213\232")   .. v188 ;buyRod(v189.B_C,v189.B_C.Position);break;end end break;end end end return;end end end if (v208==(0 -0)) then v209=game.ReplicatedStorage.playerstats[game.Players.LocalPlayer.Name].Stats;v210=(v209:FindFirstChild(v7("\221\168\204\211\96","\110\190\199\165\189\19\145\61")) and v209.coins.Value) or (362 -(112 + 250)) ;v208=1;end break;end end end end end end);end end);spawn(function() while task.wait() do pcall(function() if (v11==true) then if  not v16.playerstats[game.Players.LocalPlayer.Name]:FindFirstChild(v7("\220\248\166\35","\80\142\151\194")):FindFirstChild(v7("\55\212\126\72\6\200\99\12\49\201\115","\44\99\166\23")) then if (game:GetService(v7("\78\242\57\58\58\167\125\227\44\50\0\176\115\229\40\49\54","\196\28\151\73\86\83")).playerstats[v18.Name].Stats.coins.Value>=(59797 + 90203)) then if getgenv().Setting[v7("\213\2\59\29","\22\147\99\73\112\226\56\120")][v7("\137\96\231\230\153\248\71\237\241","\237\216\21\130\149")][v7("\182\92\86\91\181\199\74\194\124\80\91","\62\226\46\63\63\208\169")] then buyRodV_2(Vector3.new( -(3717 -2233), -(128 + 95), -2194),Vector3.new( -(768 + 716), -223, -(1641 + 553)));v51.Text=v7("\165\59\64\154\22\3\40\30\209\11\92\135\26\3\59\30\215\22\81\195","\62\133\121\53\227\127\109\79");workspace.world.interactables[v7("\36\6\59\241\211\160\182\80\38\61\241","\194\112\116\82\149\182\206")].purchaserompt.Enabled=true;end elseif (game:GetService(v7("\11\173\92\20\201\225\15\45\173\72\43\212\237\28\56\175\73","\110\89\200\44\120\160\130")).playerstats[v18.Name].Stats.coins.Value<=(74375 + 75625)) then local v239=0 + 0 ;while true do if ((1414 -(1001 + 413))==v239) then v51.Text=v7("\235\226\94\82\76\10\15\95\162\199\78\72\87\10\9\66\175\131","\45\203\163\43\38\35\42\91");game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame=CFrame.new( -(8569 -4726),1015 -(244 + 638) ,1032 -(627 + 66) );v239=1;end if (v239==(2 -1)) then farmCoins();break;end end end elseif  not v16.playerstats[game.Players.LocalPlayer.Name]:FindFirstChild(v7("\224\138\216\48","\52\178\229\188\67\231\201")):FindFirstChild(v7("\21\83\89\0\242\82\55\97\115\95\0","\67\65\33\48\100\151\60")) then local v227=0;local v228;while true do if ((602 -(512 + 90))==v227) then v228=0;while true do if (v228==(1907 -(1665 + 241))) then farmCoins();break;end if (v228==(717 -(373 + 344))) then v51.Text=v7("\159\198\187\204\252\159\211\188\209\247\218\233\186\152\193\208\227\238","\147\191\135\206\184");game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame=CFrame.new( -3843,60 + 73 ,339);v228=1 + 0 ;end end break;end end end end end);end end);spawn(function() while task.wait() do pcall(function() local v156=0;local v157;local v158;local v159;local v160;local v161;local v162;local v163;local v164;while true do if (v156==(2 -1)) then v159=v158:FindFirstChild(v7("\4\70\247\3","\174\86\41\147\112\19"));v160=v158.Stats.coins;v156=2 -0 ;end if (v156==(1099 -(35 + 1064))) then local v212=0 + 0 ;while true do if (v212==(2 -1)) then v156=1 + 0 ;break;end if (v212==(1236 -(298 + 938))) then v157=game.Players.LocalPlayer;v158=game:GetService(v7("\182\45\182\205\209\80\179\144\45\162\242\204\92\160\133\47\163","\210\228\72\198\161\184\51")).playerstats[v157.Name];v212=1260 -(233 + 1026) ;end end end if (v156==(1670 -(636 + 1030))) then if v163 then if (v164 and (v164~="") and (v163.Value~=v164)) then if  not v162 then if (v160.Value>=11000) then local v254=0 + 0 ;local v255;while true do if (v254==(0 + 0)) then v255=0 + 0 ;while true do if ((0 + 0)==v255) then v157.Character.HumanoidRootPart.CFrame=CFrame.new( -(1153 -(55 + 166)),226, -991);pcall(function() workspace.world.npcs.Merlin.Merlin.power:InvokeServer();end);break;end end break;end end else local v256=game:GetService(v7("\63\52\37\113\4\125\12\37\48\121\62\106\2\35\52\122\8","\30\109\81\85\29\109")).playerstats[game.Players.LocalPlayer.Name].Inventory;for v269,v270 in ipairs(v256:GetChildren()) do if string.find(v270.Name,v7("\205\116\88\191\53","\156\159\17\52\214\86\190")) then return;end end v51.Text=v7("\136\238\175\177\167\225\186\252\141\224\180\178\189\175\169\179\238\205\168\165\238\221\184\176\167\236","\220\206\143\221");v157.Character.HumanoidRootPart.CFrame=CFrame.new( -3843,133,66 + 273 );farmCoins();end elseif (((v10(v8.TimeOfDay)>=v10(v7("\214\45\119\71\136\150\130\214","\178\230\29\77\119\184\172"))) and (v10(v8.TimeOfDay)<=v10(v7("\165\232\80\72\39\162\165\238","\152\149\222\106\123\23")))) or (v10(v8.TimeOfDay)>=v10(v7("\140\126\172\19\229\135\118\166","\213\189\70\150\35")))) then local v259=0 + 0 ;local v260;local v261;while true do if ((11 -8)==v259) then wait(300.5 -(36 + 261) );v260=game.Players.LocalPlayer;v259=4;end if (v259==(6 -2)) then v261=v260.Character and v260.Character:FindFirstChild(v7("\17\179\184\40\132\54\190\196","\160\89\198\213\73\234\89\215")) ;if v261 then local v286=1368 -(34 + 1334) ;local v287;while true do if (v286==(0 + 0)) then v287=0 + 0 ;while true do if (v287==0) then v261:UnequipTools();for v298,v299 in ipairs(v260.Backpack:GetChildren()) do if (v299:IsA(v7("\124\126\187\242","\165\40\17\212\158")) and v299.Name:lower():find("T")) then v261:EquipTool(v299);break;end end break;end end break;end end end break;end if (v259==(1283 -(1035 + 248))) then v157.Character.HumanoidRootPart.CFrame=CFrame.new(1311, -802, -(104 -(20 + 1)));v51.Text=v7("\110\64\96\7\15\112\122\11\71\84\122\28\15","\104\47\53\20")   .. v164   .. v7("\227\88\142\92\136\29\170\72\132\18\168\79\145\67\133","\111\195\44\225\124\220") ;v259=1 + 0 ;end if (v259==(321 -(134 + 185))) then if v261 then local v288=0;while true do if ((1133 -(549 + 584))==v288) then v261:UnequipTools();for v296,v297 in ipairs(v260.Backpack:GetChildren()) do if (v297:IsA(v7("\13\124\118\77","\174\89\19\25\33")) and v297.Name:lower():find(v7("\61\23\94\71\244","\107\79\114\50\46\151\231"))) then v261:EquipTool(v297);break;end end break;end end end Click_Buy();v259=3;end if (v259==(686 -(314 + 371))) then v260=game.Players.LocalPlayer;v261=v260.Character and v260.Character:FindFirstChild(v7("\240\83\13\114\165\164\209\66","\203\184\38\96\19\203")) ;v259=6 -4 ;end end else local v262=968 -(478 + 490) ;local v263;while true do if (v262==(0 + 0)) then v263=1172 -(786 + 386) ;while true do if (v263==(0 -0)) then v51.Text=v7("\195\216\26\62\47\235\222\72\16\41\236\215\27\115\17\228\208\28\115\18\236\212\13","\70\133\185\104\83");v157.Character.HumanoidRootPart.CFrame=CFrame.new( -(5222 -(1055 + 324)),1473 -(1093 + 247) ,339);v263=1 + 0 ;end if ((1 + 0)==v263) then farmCoins();break;end end break;end end end end elseif (v160.Value>=(595526 -445526)) then if getgenv().Setting[v7("\34\68\86\39","\169\100\37\36\74")][v7("\49\146\167\67\20\199\144\95\4","\48\96\231\194")][v7("\252\72\7\41\28\214\187\195\250\85\10","\227\168\58\110\77\121\184\207")] then local v245=0 -0 ;local v246;while true do if (v245==(0 -0)) then v246=0;while true do if (v246==(0 -0)) then buyRodV_2(Vector3.new( -(528 + 956), -(858 -635), -(7562 -5368)),Vector3.new( -(1119 + 365), -(569 -346), -(2882 -(364 + 324))));workspace.world.interactables[v7("\79\46\182\68\180\213\101\229\73\51\187","\197\27\92\223\32\209\187\17")].purchasePrompt.Enabled=true;break;end end break;end end end elseif ((v15==true) and v163) then local v247=0 -0 ;local v248;while true do if (v247==(0 -0)) then v248=0 + 0 ;while true do if (v248==(0 -0)) then v51.Text=v7("\37\94\209\246\10\81\196\187\32\80\202\245\16\31\215\244\67\125\214\226\67\107\209\242\7\90\205\239\67\109\204\255","\155\99\63\163");v157.Character.HumanoidRootPart.CFrame=CFrame.new( -(6154 -2311),403 -270 ,339);v248=1269 -(1249 + 19) ;end if (v248==1) then farmCoins();break;end end break;end end end if (v163.Value==v164) then local v222=0 + 0 ;local v223;while true do if (v222==0) then v223=0 -0 ;while true do if (v223==(1086 -(686 + 400))) then v51.Text=v7("\164\208\179\128\176\138\133\145\130\130\176\138\145","\228\226\177\193\237\217");v157.Character.HumanoidRootPart.CFrame=CFrame.new( -(3016 + 827),362 -(73 + 156) ,2 + 337 );v223=812 -(721 + 90) ;end if (v223==(1 + 0)) then farmCoins();break;end end break;end end end break;end if ((9 -6)==v156) then local v213=0;while true do if ((471 -(224 + 246))==v213) then v156=5 -1 ;break;end if (v213==(0 -0)) then v163=v159 and v159:FindFirstChild(v7("\58\191\121\224\14\140\26\237\66\235\15","\226\110\205\16\132\107")) ;v164=getgenv().Setting[v7("\205\194\242\212","\33\139\163\128\185")][v7("\102\77\1\205\67\24\54\209\83","\190\55\56\100")][v7("\115\161\63\22\18\237\231\22\231\124\42\1\234\247\83\161\40\94\33\236\247\22\230","\147\54\207\92\126\115\131")];v213=1;end end end if (v156==(1 + 1)) then v161=v157:FindFirstChild(v7("\121\1\142\0\53\14\18\160","\203\59\96\237\107\69\111\113"));v162=v161 and v161:FindFirstChild(v7("\1\24\175\233\48\254\195\100\36\169\237\56\243","\183\68\118\204\129\81\144")) ;v156=1 + 2 ;end end end);end end);spawn(function() while wait(111 + 39 ) do if (v9==true) then local v190=0 -0 ;local v191;while true do if (v190==(0 -0)) then v191=513 -(203 + 310) ;while true do if (v191==0) then game:service(v7("\2\185\49\242\33\177\47\207\58\160\54\242\25\177\45\231\51\181\49","\134\84\208\67")):SendKeyEvent(true,v7("\32\188\135\95\22","\60\115\204\230"),false,game);wait(1993.5 -(1238 + 755) );v191=1;end if (v191==1) then game:service(v7("\209\51\249\100\242\59\231\89\233\42\254\100\202\59\229\113\224\63\249","\16\135\90\139")):SendKeyEvent(false,v7("\103\100\7\48\75","\24\52\20\102\83\46\52"),false,game);break;end end break;end end end end end);spawn(function() while wait() do if (getgenv().Setting[v7("\226\46\51\41","\111\164\79\65\68")][v7("\245\220\151\202\39\228\193","\138\166\185\227\190\78")][v7("\249\113\192\59","\121\171\20\165\87\50\67")]==true) then game:GetService(v7("\244\61\169\58\176\1\199\44\188\50\138\22\201\42\184\49\188","\98\166\88\217\86\217")):WaitForChild(v7("\243\224\124\15\146\207","\188\150\150\25\97\230")):WaitForChild(v7("\200\140\90\14\10\228\212\128\76\10\9\233","\141\186\233\63\98\108")):FireServer(7 + 93 ,true);end end end);
