<template>
  <div class="slidev-layout four-tiles">
    <!-- Header Section -->
    <div class="header-section text-center pt-4 pb-2">
      <h1 class="text-2xl font-bold mb-2">
        <slot name="title" />
      </h1>
      <div class="text-base text-gray-200">
        <slot name="subtitle" />
      </div>
    </div>

    <!-- Four Tiles Grid -->
    <div class="tiles-section p-4">
      <div class="grid grid-cols-2 gap-3 h-full">
        <!-- Tile 1 -->
        <div class="tile flex flex-col items-center justify-center text-center p-3">
          <div class="icon-container mb-2">
            <slot name="icon1">
              <div class="text-4xl">🔧</div>
            </slot>
          </div>
          <div class="tile-content">
            <slot name="tile1" />
          </div>
        </div>

        <!-- Tile 2 -->
        <div class="tile flex flex-col items-center justify-center text-center p-3">
          <div class="icon-container mb-2">
            <slot name="icon2">
              <div class="text-4xl">⏰</div>
            </slot>
          </div>
          <div class="tile-content">
            <slot name="tile2" />
          </div>
        </div>

        <!-- Tile 3 -->
        <div class="tile flex flex-col items-center justify-center text-center p-3">
          <div class="icon-container mb-2">
            <slot name="icon3">
              <div class="text-4xl">🔧</div>
            </slot>
          </div>
          <div class="tile-content">
            <slot name="tile3" />
          </div>
        </div>

        <!-- Tile 4 -->
        <div class="tile flex flex-col items-center justify-center text-center p-3">
          <div class="icon-container mb-2">
            <slot name="icon4">
              <div class="text-4xl">✅</div>
            </slot>
          </div>
          <div class="tile-content">
            <slot name="tile4" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.four-tiles {
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: column;
}

.header-section {
  flex-shrink: 0;
}

.header-section h1 {
  color: white;
}

.tiles-section {
  flex: 1;
  display: flex;
  flex-direction: column;
}

.tiles-section .grid {
  flex: 1;
  max-height: calc(100vh - 120px);
}

.tile {
  background: rgba(255, 255, 255, 0.1);
  border-radius: 8px;
  backdrop-filter: blur(10px);
  border: 1px solid rgba(255, 255, 255, 0.2);
  transition: transform 0.2s ease, background 0.2s ease;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.tile:hover {
  transform: translateY(-2px);
  background: rgba(255, 255, 255, 0.15);
}

.icon-container {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-shrink: 0;
}

.tile-content {
  font-size: 0.8rem;
  line-height: 1.3;
  text-align: center;
  flex: 1;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.tile-content h3 {
  font-size: 0.9rem;
  font-weight: 600;
  margin-bottom: 0.3rem;
  color: white;
}

.tile-content p {
  color: rgba(255, 255, 255, 0.9);
  font-size: 0.75rem;
}
</style>
