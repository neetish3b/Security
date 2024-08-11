    getUniquePlatforms = () => {
        const { platforms } = this.state;
        // Remove duplicates based on 'id'
        const uniquePlatforms = [...new Map(platforms.map(platform => [platform.id, platform])).values()];
        return uniquePlatforms;
    };

    onFilterChanges = (e) => {
        this.setState({ selectedPlatform: e.value });
    };


 const data = [
            { id: '1', platformName: 'Platform A' },
            { id: '2', platformName: 'Platform B' },
            { id: '3', platformName: 'Platform C' }
        ];
