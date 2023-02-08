# Dependencies
- docker (docker-engine or docker-desktop)
- docker-compose

# Setup Instruction

## 1. Clone this repository with submodules
```
git clone --recurse-submodules https://github.com/thekitp/librespeed-playground.git
```

## 2. Create persistence storage
```
docker volume create librespeed-speedtest-storage
```

## 3. Build service
```
docker-compose build
```

## 4. Start service
```
docker-compose up -d
```

## 5. Create database
```
docker-compose run create-database
```

# Usage

- Main speed test page is http://localhost:41800/
- Stats page is http://localhost:41800/results/stats.php (default password is `12341234`)
- Database admin ui http://localhost:41801/