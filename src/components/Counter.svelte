<div class="counter" on:click="set({ count: count + 1 })">
    <div class="counter__number">
        {count}
    </div>
</div>

<style>
.counter {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 15rem;
    height: 15rem;
    background-color: #fff;
    border: 1px solid #fcfcfc;
    border-radius: 100%;
    box-shadow: 2px 2px 10px rgba(0, 0, 0, .1);
    cursor: pointer;
}

.counter__number {
    font-size: 6rem;
}
</style>

<script>
export default {
    data() {
        return {
            count: 0
        };
    }
}
</script>
