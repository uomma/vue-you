<script>
export default {
    name: 'Search'
}
</script>

<template>
    <div class="container">
        <form>
            <div class="row justify-content-center">
                <div class="mb-3 col-12 col-sm-auto">
                    <label for="search-card" class="form-label d-none">Search</label>
                    <input type="text" class="form-control" id="search-card" aria-describedby="emailHelp"
                        placeholder="search card">
                </div>
                <div class="mb-3col-12 col-sm-auto">
                    
                    <select class="form-select" id="search-card">
                        <option selected>select card</option>
                        <option value="1">One</option>
                        <option value="2">Two</option>
                        <option value="3">Three</option>
                    </select>
                </div>
                <div class="mb-3col-12 col-sm-auto">
                    <button type="submit" class="btn btn-primary">Search</button>

                </div>

            </div>
        </form>
    </div>
</template>



<style lang="scss" scoped></style>