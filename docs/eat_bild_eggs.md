```mermaid

flowchart TB

subgraph "第1階層"

    eat_egg["ゆで卵を食べる"]

end

subgraph "第2階層"
    bay_egg["卵を買う"]
    cook_egg["ゆで卵を作る"]
    prepare_eat["食べる準備をする"]

end


subgraph "第3階層"

    bank["銀行でお金をおろす"]
    super["スーパーで卵を買う"]

    washegg["卵を洗う"];
    yudemizu["お湯を沸かす"]
    yudetama["卵をゆでる"]

    hukkin["腹筋して腹を減らす"]
    crack["殻をわる"]
    salt["塩を振る"]

end


%% 第2階層

eat_egg--->bay_egg;
eat_egg--->cook_egg;
eat_egg--->prepare_eat;


%% 第3階層

bay_egg--->bank;
bay_egg--->super;

cook_egg--->washegg;
cook_egg--->yudemizu;
cook_egg--->yudetama;

prepare_eat--->hukkin;
prepare_eat--->crack;
prepare_eat--->salt;

 

```